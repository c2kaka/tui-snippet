---
prefix: t-select
description: tui select component
scope: html
---

```html
<tui-select
 ${1: name=""}
 ${2: placeholder=""}
 ${3: [(ngModel)]=""}
 ${4: (ngModelChange)="onSelectChange($event)"}
 ${5: allowClear}
>
  <tui-select-option
    *ngFor="let option of objectOptions"
    [value]="option.value"
    [disabled]="option.disabled"
  >
    {{ option.label }}
  </tui-select-option>
</tui-select>
```