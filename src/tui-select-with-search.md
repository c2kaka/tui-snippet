---
prefix: t-select-search
description: tui select component with search
scope: html
---

```html
<tui-select
 ${1: allowSearch}
 ${2: searchKey="label"}
 ${3: name=""}
 ${4: placeholder=""}
 ${5: [(ngModel)]=""}
 ${6: (ngModelChange)="onSelectChange($event)"}
 ${7: allowClear}
>
  <tui-select-option
    *ngFor="let option of objectOptions"
    [label]="option.label"
    [value]="option.value"
    [disabled]="option.disabled"
  >
    {{ option.label }}
  </tui-select-option>
</tui-select>
```