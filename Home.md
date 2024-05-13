---
cssclasses:
  - dashboard
---
# Valut Info
---
### Project
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
