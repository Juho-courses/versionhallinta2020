# 04 - Muutosten käsittely

## Ennakkotehtävä

Selvitä itsellesi, miten tutkitaan repositoryn historiaa ja mitä eri tapoja on hallita muutoksia.

## .gitignore

Tiedosto, jolla kerrotaan gitille tiedostot ja hakemistot joita **ei** seurata.

## Komennot

- `git log`
	- Repositoryn historian tarkastelu
- `git diff <filename>`
	- Muutosten vertailu
- `git restore <filename>`
	- Niiden muutosten poistaminen tiedostosta, joita **ei** olla commitoitu.
- `git restore --staged <filename>`
	- Tiedoston poistaminen `staged`-tilasta (muutokset säilyvät)
- `git revert <commit_hash>`
	- Peruuttaa määritellyn commitin tuomat muutokset
	- Ei kirjoita historiaa uudestaan, vaan tekee uuden commitin
- `git reset --hard HEAD^`
	- Palaa yhden commitin taaksepäin ja poistaa sen tekemät muutokset
	- **Käytä varoen**, sillä kirjoittaa historian uudestaan
