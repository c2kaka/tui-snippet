---
prefix: t-multi-select
description: tui multi select component
scope: html
---

```html
<tui-select
 ${1: name=""}
 ${2: placeholder=""}
 ${3: mode="multiple"}
 ${4: [(ngModel)]=""}
 ${5: (ngModelChange)="onSelectChange($event)"}
 ${6: allowClear}
>
  <tui-select-option-all></tui-select-option-all>
  <tui-select-option
    *ngFor="let option of objectOptions"
    [value]="option.value"
  >
    <span>{{ option.label }}</span>
  </tui-select-option>
</tui-select>
```