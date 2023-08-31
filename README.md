 # cd
Hierbij mijn verslag over het project CD. Deze hb ik gemaakt met behulp van een flask app en Digital Ocean. De bedoeling van het project is: bij een wijziging in Flask-app, en na het pushen en/of uploaden van het project naar github, wordt mijn project op mijn virtuele server ook gewijzigt.

# 3 componenten die gebruikt zijn
## Github actions
In Github actions heb ik een main.yml bestand gemaakt.
in dit bestand staan de acties die uitgevoerd worden. In dit geval zijn dat 2 acties. Test en Deploy acties.
Pytest doet de eerste fase en wanneer de test compleet is kan mijn project door eerst in te loggen in mijn virtuele server uiteinelijk aangeroepen worden (Deploy fase)
## SSH keys
Om in te loggen op je server maak je gebruik van een speciale sleutel. Deze sleutel heb ik gegeneerd in github. Ik heb een private en een public key gegenereerd. Mijn public-key staat in mijn map .ssh directory in de map: authorized_keys.
En mijn private-key staat onder secrets in Github. Ik had wel moeite om te begrijpen hoe het allemaal werkte en hoe ik uiteindelijk alles moest genereren en opslaan.
## Github-secrets
In Github-secrets heb je de mogelijkheid om je inloggegevens zoals je username, ip adressen en keys op te slaan. Na een paar Youtube videos te hebben bekeken kwam ik er achter hoe dit in elkaar zit. 

# Eindconclusie
Dit is een pittige opdracht waarbij er veel uitgezocht diende te worden. Uiteinelijk had ik stap 1 voor elkaar door de opdracht werkende te krijgen in VS code. En daarna kwam stap 2 actions om de hoek kijken. Hier heb ik toch wel de meeste tijd in zitten samen met die SSh key en Secrets. Uiteindelijk vind ik het ook wel weer mooi om te zien dat een opdracht zoals deze op een simpele manier connectie maakt met een virtuel server en daar de wijzigingen door stuurt. Na veel zoeken en uitvogelen ben ik blij dat de CD opdracht werkt.