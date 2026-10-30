# Projekti reeglid

## Projekt
- See on õppeprojekt: üks brauserirakendus failis index.html (HTML, CSS ja JavaScript samas failis).
- Ära lisa väliseid teeke, raamistikke, build-samme ega teisi faile, kui ma seda ei palu.
- Kasutajaliidese tekst ja koodi kommentaarid on eesti keeles.
- HTML algab <!doctype html> deklaratsiooniga; lisa lang="et", UTF-8 kodeering ja mobiili viewport-seadistus.
- Kasuta ainult väljamõeldud andmeid. Ära küsi ega salvesta isikuandmeid.
- localStorage'i kasutus alati try/catch-iga. Kontrolli loetud andmete kuju ja piire; salvestamise tõrge ei tohi kogu rakendust peatada.
- Kasutaja teksti kuva textContent abil; ära tõlgenda seda HTML-i ega JavaScriptina. Ära kasuta eval-i ega Function-konstruktorit.
- Ära lisa saladusi, API-võtmeid ega loata väliseid võrgupäringuid.
- Juhisefailid ja avaldamisel automaatselt loodav väljundkaust on ühe rakendusfaili reegli erandid. Ainus käsitsi muudetav rakendusfail on juurkausta index.html.

## Töövoog
- Tee korraga ainult see muudatus, mida palun. Ära paranda muud koodi omal algatusel.
- Enne suuremat muudatust kirjelda lühidalt plaan.
- Loe enne muutmist asjakohast olemasolevat koodi. Kontrolli sisendeid, piirväärtusi ja ootuspäraseid veaseisundeid; ära peida vigu tühja catch-plokiga.
- Lähtu ülesande valmisoleku kriteeriumidest ja kontrolli ka seotud olemasolevaid funktsioone.
- Kasuta olemasolevaid kontrollvahendeid. Ära nimeta testituks seda, mida sa ei proovinud; erista mõõtmist hinnangust.
- Kokkuvõttes ütle, mida muutsid, mida kontrollisid ja mis oli tulemus, mida kasutaja peab ise proovima ning mis jäi lahendamata.
- Ära tee commit'i ega push'i, kui ma seda ei palu. Enne taastamist selgita võimalikku andmekadu ja küsi kinnitust.
- Ära käivita terminalikäske, mis kustutavad faile või paigaldavad pakette.

## Kujundus (Refactoring UI põhimõtted)
- Vahede lähtepunktid: 4, 8, 12, 16, 24, 32, 48, 64, 96 px.
- Fondisuurused ainult skaalast: 12, 14, 16, 18, 20, 24, 30, 36, 48 px. Sisutekst 16 px ja reavahe 1.5; suured pealkirjad reavahe 1.1–1.25.
- Värvid CSS-muutujatena: 8–10 tooni halli (mitte puhas must), üks põhivärv 5–10 tooniga, eraldi värvid õnnestumisele, hoiatusele ja veale.
- Hierarhia värvi ja kaaluga, mitte ainult suurusega: põhitekst tume, teisene tekst keskmine hall, abiinfo hele hall.
- Nuppude hierarhia: üks peamine tegevus (täidetud), teisesed (kontuur), harvad tegevused (lingi stiilis). Kustutamine ei ole automaatselt suur punane nupp.
- Eralda elemente vahe, taustatooni või varjuga; ääriseid kasuta säästlikult.
- Varjud kahest osast (suur pehme + väike tume). Mida kõrgemal element on, seda suurem ja pehmem vari.
- Tekstirea pikkus 45–75 märki. Ära tsentreeri pikka teksti.
- Ära edasta infot ainult värviga: lisa tekst, ikoon või kuju.
- Tühjad olekud on kujundatud ja juhatavad esimese sammu juurde.
- Tegevusteks kasuta <button>, linkimiseks <a>. Fookus peab olema nähtav, väljad sildistatud ja veateated arusaadavad. Puuteala eesmärk on vähemalt 44 × 44 px; leht töötab telefonis ja klaviatuuriga. Arvesta prefers-reduced-motion eelistust.