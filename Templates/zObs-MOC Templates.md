---
noteType: MOC
tags:
  - MOC
---
==[[INDEX]]==

```dataview
TABLE WITHOUT ID
	file.link AS "Note",
	fm AS "Properties",
	tags AS "Tags"
WHERE 
	contains(file.frontmatter, "noteType")
	OR contains(file.etags, "MOC")
	OR contains(noteType, "MOC")
SORT default(file.name, "") ASC,
	file.name DESC
FLATTEN file.frontmatter AS fm

```

```ad-note
title: zObs

For back-end automation (template/retrieval) use

```
