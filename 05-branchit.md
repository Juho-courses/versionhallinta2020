# 05 - Branchit

## Ennakkotehtävä

Git repositoryn historia voidaan mieltää puurakenteisena. Selvitä, miten puunoksia (branch) käytetään hyödyksi ohjelmistoprojektissa.

## Komentoja

### Branch

- Branchin luominen
	- `git branch <nimi>`
	- esimerkiksi `git branch feat-1`
- Branchiin vaihtaminen
	- `git checkout <nimi>`
	- esimerkiksi `git checkout feat-1`
- Luo uuden branchin ja vaihtaa siihen
	- `git checkout -b <nimi>`
	- esimerkiksi `git checkout -b feat-2`
- Branchien listaus
	- `git branch -a`
- Kahden branchin mergeäminen
	- `git merge <nimi>`
	- esimerkiksi `git merge feat-2`, mergeää `feat-2`-branchin siihen branchiin mikä on aktiivisena kun ajat komennon

### Log

- Login piirtäminen graafina
	- `git log --oneline --graph`

### Commit

- `git commit -am 'viesti'`
	- `git add`aa kaikki tiedostot (`-a`) ja tekee commitin
	- Käytä varoen! Vain silloin kun tiedän varmasti, että committiin ei mene mukaan ei-haluttuja muutoksia.

