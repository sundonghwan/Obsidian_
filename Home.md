---
cssclasses:
  - dashboard
---
# Valut Info
- Recent file updates

```dataview

TABLE dateformat(file.mtime, "yyyy/MM/dd") AS "Last Modified"

WHERE date(today) - file.mtime <= dur(7 days) SORT file.mtime DESC

```
