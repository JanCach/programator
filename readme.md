honzovy-vtipy.netlify.app
===================

HTML a CSS
------------------
Kód pro stránky jsem psal v **html** a nastyloval v **css**

Struktura stránek a šablona
------------------------------------
Na úvodní stránce jsou tlačítka s odkazem na jednotlivé kategorie vtipů (6 dalších stránek) a na hádanky (1 další stránka) 

Stránky pro jednotlivé kategorie vtipů a pro hádanky jsou založeny na jednotné šabloně (ve složce _includes) 

Použil jsem šablonovací engine **nunjucks** (njk) ![obrázek nunjucks](/images/njk.jpg) a generátor statických webů **eleventy/11ty** ![obrázek eleventy](/images/eleventy.jpg)

Netlify
---------
Vzhledem k použití šablony jsem místo GitHub Pages využil pro publikování stránek službu [Netlify](https://netlify.com) ![obrázek netlify](/images/netlify.jpg)

Responzivita
-----------------
Rozložení stránek a menu je responzivní (pomocí @media) s využitím **gridu**

Barvy a písmo
-------------------
Použité barvy jsem uložil do proměnných, abych je v případě potřeby mohl snadno změnit 

Pro podbarvení tlačítek a pozadí jednotlivých vtipů jsem použil selektor :nth-child() 

Pro podbarvení v menu dle aktuální stránky jsem v šabloně použil podmínku {{ 'menu__item--active' if page.fileSlug==='...' }}

Čitelnost barvy písma vzhledem k pozadí tlačítek jsem ověřil pomocí [contrast checkeru](https://webaim.org/resources/contrastchecker/)

Font pro písmo jsem vybral Rubik na [Google Fonts](https://fonts.google.com/)

Favicon
-----------
![ikona stránek](/favicon/favicon.ico) Vektorový obrázek pro favicon jsem nadesignoval a sestavil ve vektorovém editoru [Vectr](vectr.com) 

Pro vygenerování faviconu jsem následně použil [RealFaviconGenerator](https://realfavicongenerator.net/)