# PCS1-kontroly
Sběr záznamů PCS1

Script má dvě části.
1. Zpracuje informace PCS1 v centru. Zdrojem záznamů jsou sebrané logy vybraných stanic ve formátu txt.
2. Zpracuje informace PCD1 ZU. Zdrojem záznamů jsou logy úřadů ve formátu csv.

Při spuštění script nabízí možnost sebrat záznamy o PCS1 z úřadů, centra nebo ze všech stanic.
Před sběrem se script ještě dotáže na rok a měsíc od kdy má zpracovávat informace. 
Následně dojde ke zpracování. 

Fungování:
V prvé řadě zmapuje jednotlivá úložiště (uložiště centra a úřadů se různí). U ZU dochází k rozbalení zipových souborů s logy do složky 
mytemp vytvořené scriptem. Z výsledných csv dokumentů jsou posléze sbírány záznamy PCS1. U stanic centra jsou záznamy sbírány přímo 
z logů konkrétních stanic bez potřeby extrakce dokumentů. Informace jsou přepracovány do požadovaného tvaru a uloženy ve formátu CSV.
