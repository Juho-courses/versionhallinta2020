# 06 - Hajauttaminen

## Ennakkotehtävä

Git on toimii hajautetusti (distributed). Selvitä miten työskennellään jossain muualla sijaitsevan (remote) repositoryn kanssa. Millaisia työskentelymalleja (workflow) remoten kanssa työskentely mahdollistaa?

## Komentoja

### Branch

- Branchin uudelleen nimeäminen
	- `git branch -M <uusi_nimi>`

### Clone

- Repositoryn kloonaaminen
	- `git clone <polku>`
	- Kloonaamiseen ei tarvitse esimerkiksi Github-tunnuksia, koska public repositoryn näkee kaikki.

### Remote
- Remoten lisääminen
	- `git remote add <nimi> <polku>`
- Listaa asetetut remotet
	- `git remote -v`

### Push / Pull
- Paikallisesti tehtyjen committien puskeminen (pushaaminen) remoteen
	- `git push <remoten_nimi> <branchin_nimi>`
- Remotesta muutosten hakeminen (pullaaminen) paikalliseen repositoryyn
	- `git pull <remoten_nimi> <branchin_nimi>`
	- `git pull` on shorthand `git fetch` ja `git merge` yhdistelmälle

## Käsitteitä

### Fork

Githubissa uuden repositoryn luominen toisen repon pohjalta. Ikään kuin copy-paste -- historia säilyy.

### Pull request (PR)

Muutosten tarjoaminen omasta repositorystä toiseen repoon. Repoilla pitää olla yhteinen historia, eli forkkaamalla luodusta reposta voi tarjota muutokset alkuperäiseen repositoryyn.

Jos (kun!) tekee PR:n siten, että muutokset elävät yhdessä omassa branchissa, PR seuraa sitä branchia. Eli jos tekee muutoksia branchiin ja puskee commitit, PR päivittyy automaattisesti.