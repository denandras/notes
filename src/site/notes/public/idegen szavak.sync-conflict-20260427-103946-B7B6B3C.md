```dataview
TABLE idegenszo AS "Szó", file.name AS "Forrás"
FROM ""
WHERE idegenszo AND !fileExists("public/" + replace(idegenszo, "[[", "").replace("]]", "") + ".md")
SORT file.name ASC
```