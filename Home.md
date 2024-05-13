---
cssclasses:
  - dashboard
---
# Valut Info
- Recent file updates

```dataview

TABLE dateformat(file.mtime, "yyyy/MM/dd") AS "<span>Last Modified</span>"

WHERE date(today) - file.mtime <= dur(7 days) SORT file.mtime DESC

```
