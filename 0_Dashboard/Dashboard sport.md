#  Programme Sport

##  To-Do
```dataview
TABLE WITHOUT ID
  file.link AS "Séance",
  date AS "Date prévue",
  type_seance AS "Programme",
    duree_min + " min" AS "Durée"
FROM #seance 
WHERE termine = false
SORT date ASC
```

---



##  Historique des séances terminées
```dataview
TABLE WITHOUT ID
  file.link AS "Séance",
  date AS "Date",
  type_seance AS "Type",
  duree_min + " min" AS "Durée"
FROM #seance
WHERE termine = true
SORT date DESC
```
