# wfhungary.hu – Workflow Hungary Kft. landing page

Statikus, egyoldalas landing page, GitHub Pages-re. Nincs build lépés, nincs függőség.

## Fájlok
- `index.html` – a teljes oldal (HTML + CSS + egy kis JS a mobilmenühöz)
- `CNAME` – az egyedi domain (wfhungary.hu) a GitHub Pages számára
- `images/` – a partnerlogók (átlátszó hátterű PNG-k); új logót ide tegyél, és az `index.html` Partnereink részében hivatkozz rá

## Szerkesztés
Az `index.html`-ben minden cserélendő részt `<!-- SZERKESZTENDŐ -->` megjegyzés jelöl:
hero szöveg, tevékenységek, cégbemutató, számok, partnerek, elérhetőségek, cégadatok.

## Közzététel GitHub Pages-en
1. Hozz létre egy új repót (pl. `wfhungary.hu`), és töltsd fel a mappa teljes tartalmát (`index.html`, `CNAME`, `images/`).
2. Repo → **Settings → Pages** → Source: *Deploy from a branch*, Branch: `main`, mappa: `/ (root)`.
3. A **Custom domain** mezőben a `wfhungary.hu` megjelenik (a CNAME fájlból), pipáld be az **Enforce HTTPS**-t, amint elérhető.

## DNS beállítás (a domain szolgáltatónál)
Gyökérdomainhez (`wfhungary.hu`) négy **A** rekord:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```
A `www` aldomainhez egy **CNAME** rekord: `<github-felhasználónév>.github.io`

A DNS változás érvénybe lépése akár 24 óra is lehet.
