# VASTAUKSET AVOIMIIN HARJOITUSTEN KYSYMYKSIIN

## PAIKALLINEN GIT

__Harjoitus 2__

Kysymys 8: git log ja git log --stat näyttävät tietoja commiteista. Käyttäjä näkee commit viestin, commitin tekijan, commit hashin sekä ajan jolloin commit on tehty. Sillä näkee missä ollaan tällä hetkellä menossa (head) ja mitä aiemmin ollaan commitoitu kelaamalla alaspäin.

--stat lisää tähän vielä sen, että käyttäjälle näytetään mihin tiedostoihin commit on koskenut ja mitä commitissa on tapahtunut.

__Harjoitus 3__

Kysymys 3: Untracked tiedostot eivät kokonaan poistuneet. Ne piti joko poistaa tai lisätä käsin. Poistin itse untrackedit git clear -f komennolla, joka poistaa untrackedit forcella.
Kysymys 4: Log komentoon tuli revertin jälkeen uusi ns "commit" joka oli oikeastaan revert, jossa kerrottiin, että tietty committi revertattiin.

__Harjoitus 4__

Kysymys 5: Tyylit haarassa muutokset olivat, kun taas masterissa ei ollut. Se oli siis täysin tyylimäärittelyjä ilman.
Kysymys 7: Mergen jälkeen haarat näyttävät ohjelman osalta taas samalta. Mergellä master sai tyylimäärittelytiedostot.

## HAJAUTETTU GIT

__Harjoitus 5__

Kysymys 1: Uuden tyhjän github repon luomisen jälkeen näyttää käyttäjälle siltä, ettei repossa ole mitään tavaraa. Github ehdottaakin repon tehneelle käyttäjälle toimintatapoja, joiden avulla käyttäjä saa repoon linkitettyä kokonaan uuden paikallisen gitin tai vaihtoehtoisesti jo olemassa olevan repon. Se jakaa käyttäjälle komennot, jotka voidaan ajaa terminaalissa, jotta hosting voidaan ottaa käyttöön.

Kysymys 4: Puskemisen jälkeen remote repossa näkyy nyt puskemani master haaran sisältö. Toisen haaran, eli tyylit sisältöä ei ole saatavilla remotessa, koska sitä ei ole puskettu. Omassa lokaalissani nyt näen myös VSCODEssa esimerkiksi vasemmalta alakulmasta myös remote haarat ja niiden sisällön vaihtamalla haaraa. Nyt myös voin lokaalissa käyttää git pull tai git fetch toimintoja, jossa haen remote haaraan tulleet muutokset omaan lokaaliini.

Kysymys 6: Git fetch ei muuttanut omaa lokaaliani, mutta näytti, että muutoksia on tulossa, mitä ei ole yhdistetty. Checkouttaaminen remoten master haaraan näytti nyt lokaalissa remotesta tulevat muutokset.

Kysymys 7: Master haaraan palaamisen jälkeen git status sanoo, että "Your branch and 'origin/master' have diverged", johtuen siitä, että täytim vastauksia avoimiin kysymyksiin, ilman, että puskin niitä remoteen. Eli molemmissa "haaroissa" oli tässä tapauksessa muutoksia, joita toisessa ei ollut. Jos en avoimiin kysymyksiin olisi kirjoitellut vastauksia, olisi status suurella todennäköisyydellä ilmoittanut, että oma paikallinen haarani on x määrä committeja perässä remotea.

Kysymys 8: Omassa tapauksessani yhdistämisen (merge) jälkeen status kertoi minulle, että olen x määrä committeja edellä johtuen edelleen avoimiin kysymyksiin vastaamisesta. Kuitenkin veikkaan, että tässä haettiin taas tilannetta, jossa status olisi kertonut, että lokaali on nyt ajantasalla remoten kanssa.