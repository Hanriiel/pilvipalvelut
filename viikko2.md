# Viikko 2

## Jekyll-sivuston automatisointi GitHub Actions -toiminnoilla
Jekyll-sivuston automatisointi GitHub Actionsilla voidaan toteuttaa lisäämällä projektin GitHub-repositorioon YAML-muotoinen workflow-tiedosto, joka määrittelee CI/CD-putkiston eri vaiheet. Workflow käynnistyy esimerkiksi, kun pushataan uusi commit päähaaraan tai tehdään pull request. Tiedostossa määritellään vaiheet, kuten Jekyll-sivuston riippuvuuksien asennus, sivuston rakentaminen (jekyll build) sekä valinnaisesti testaaminen. Lopuksi workflow voi julkaista valmiin sivuston GitHub Pagesiin komennolla gh-pages. Näin jokainen päivitys saadaan automaattisesti käyttöön ilman manuaalista julkaisua.

## CI/CD-putkiston rakentaminen
CI/CD-putkiston rakentamiseen web-sovellukselle käytetään yleisesti kehitystyökaluja, kuten GitHub Actionsin lisäksi Dockeria, joka mahdollistaa ympäristöjen eristämisen ja toistettavuuden. Myös testauskirjastot (esim. Jest, Mocha) ja lintterit (esim. ESLint, Stylelint) ovat hyödyllisiä laadunvalvonnassa. Dockerin avulla voidaan määritellä tarkat riippuvuudet ja ympäristöt, ja testit voidaan automatisoida osana workflow'ta. Näiden avulla rakennettu CI/CD-putkisto parantaa tehokkuutta, varmistaa jatkuvan laadun ja nopeuttaa julkaisuprosessia, mikä on keskeistä moderneissa ohjelmistokehitysprojekteissa.
