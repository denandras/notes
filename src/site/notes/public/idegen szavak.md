```dataview
TABLE idegenszo AS "Szó", file.name AS "Forrás"
FROM ""
WHERE idegenszo AND file.name != "idegen szavak" AND !fileExists("public/" + replace(idegenszo, "[[", "").replace("]]", "") + ".md")
SORT file.name ASC
```