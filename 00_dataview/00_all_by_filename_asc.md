``` dataview
TABLE
	dateformat(file.ctime,"yyyy-MM-dd, HH:mm") AS "作成日時",
	dateformat(file.mtime,"yyyy-MM-dd, HH:mm") AS "更新日時"
FROM "01_inbox" OR "03_projects" OR "50_資料/02_notes" OR "99_diary"
SORT file.filename ASC
```
