# VASTAUKSET AVOIMIIN HARJOITUSTEN KYSYMYKSIIN

## PAIKALLINEN GIT

__Harjoitus 2__

Kysymys 8: git log ja git log --stat näyttävät tietoja commiteista. Käyttäjä näkee commit viestin, commitin tekijan, commit hashin sekä ajan jolloin commit on tehty. Sillä näkee missä ollaan tällä hetkellä menossa (head) ja mitä aiemmin ollaan commitoitu kelaamalla alaspäin.

--stat lisää tähän vielä sen, että käyttäjälle näytetään mihin tiedostoihin commit on koskenut ja mitä commitissa on tapahtunut.

__Harjoitus 3__

Kysymys 3: Untracked tiedostot eivät kokonaan poistuneet. Ne piti joko poistaa tai lisätä käsin. Poistin itse untrackedit git clear -f komennolla, joka poistaa untrackedit forcella.
Kysymys 4: Log komentoon tuli revertin jälkeen uusi ns "commit" joka oli oikeastaan revert, jossa kerrottiin, että tietty committi revertattiin.

__Harjoits 4__

Kysymys 5: Tyylit haarassa muutokset olivat, kun taas masterissa ei ollut. Se oli siis täysin tyylimäärittelyjä ilman.
Kysymys 7: Mergen jälkeen haarat näyttävät ohjelman osalta taas samalta. Mergellä master sai tyylimäärittelytiedostot.