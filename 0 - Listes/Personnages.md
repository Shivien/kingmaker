---
tags:
  - Liste
---
## Personnages non joueurs

```dataviewjs
dv.table(
	["Nom", "Factions"],
	dv.pages("#Personnage/PNJ")
		.sort(p => p.file.name)
		.map(p => [p.file.link, p.factions])
)
```
