# Stránka Slovenskej spoločnosti pre mimotelový obeh

Beží na **https://www.perfuzia.sk** cez Netlify. Netlify je napojený na tento
repozitár, takže **každý `git push` do vetvy `main` stránku automaticky zverejní**.
Netreba nič nahrávať cez FTP.

## Čo kde je

| Súbor / priečinok | Na čo je |
|---|---|
| `index.html` | hlavná stránka: banner kongresu, medzinárodná spolupráca, sponzori, kontakt |
| `o-nas.html` | text o perfuziológii a o spoločnosti |
| `stanovy.html` | odkaz na stiahnutie stanov |
| `styles.css` | vzhľad celej stránky (farby, hlavička, dlaždice, pätička) |
| `img/` | logo spoločnosti, banner kongresu, logá partnerov |
| `img/sponzori/` | logá sponzorov, každý zvlášť |
| `img/icons/` | ikony stránky pre prehliadač a mobil |
| `img/archiv/` | staré obrázky, ktoré sa už nepoužívajú (program kongresu, staré plagáty) |
| `dokumenty/` | PDF na stiahnutie |
| `favicon.ico` | ikonka v záložke prehliadača a vo vyhľadávaní |
| `robots.txt`, `sitemap.xml` | pre vyhľadávače, aby stránku našli |

## Časté úpravy

**Pridať sponzora:** obrázok loga ulož do `img/sponzori/` a v `index.html`
v sekcii „Sponzori“ pridaj riadok:

```html
<div class="sponsor"><img src="img/sponzori/nazov.png" alt="Názov firmy"></div>
```

**Vymeniť plagát kongresu:** nahraď `img/beograd.jpg` novým obrázkom
(alebo pridaj nový a uprav cestu v `index.html` v sekcii `hero-banner`).

**Fotka do hlavičky:** stačí uložiť obrázok ako `img/header.jpg`, sama sa
zobrazí vpravo v modrej hlavičke. Kým tam nie je, hlavička je len modrá.

**Zverejniť zmeny:**

```
git add -A
git commit -m "popis zmeny"
git push
```

Netlify to nasadí do pár desiatok sekúnd.
