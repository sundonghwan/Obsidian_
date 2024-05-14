---
cssclasses:
  - dashboard
---
# Valut Info
---
### 최근 문서 변경 목록
---
```dataviewjs
const cfile = dv.current().file;
const list = dv.pages(`"${cfile.folder}"`)
    .filter(b => b.file.name != cfile.name)
    .sort(b => b.file.cday)
    .map(b => b.file.link);
dv.list(list);
```


---
