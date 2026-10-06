# TK Slavia Plzeň — návrhy nového webu

Čtyři návrhy nového webu pro **TK Slavia Plzeň z.s.** (U Borského parku 2916/19, Plzeň),
náhrada za současný web [tkslaviaplzen.cz](https://tkslaviaplzen.cz/).

**Náhled online:** https://petrluxa.github.io/tkslaviaplzen-navrhy/

Zadání: **luxusní · živé · klub s velkou tradicí**, plus tři konkrétní požadavky —
přihláška do klubu, sekce trenéři a přehledný ceník.

## Varianty

Otevři [`index.html`](index.html) — galerie všech čtyř variant s porovnáním.

| | Varianta | Charakter |
|---|---|---|
| 01 | [`01-kronika.html`](01-kronika.html) | Tmavá klubová zeleň, kartáčované stříbro, tenisově žlutý akcent. Serifová typografie, velká časová osa a zeď odchovanců. Nejluxusnější. |
| 02 | [`02-antuka.html`](02-antuka.html) | Světlá magazínová — krémová, antuková terakota, klubová zeleň. Luxus dělá prostor a jemné linky. |
| 03 | [`03-extraliga.html`](03-extraliga.html) | Moderní sportovní — bílá, hluboká zeleň, žlutá jiskra, velká bloková typografie a obří čísla. Nejživější. |
| 04 | [`04-kronika-svetla.html`](04-kronika-svetla.html) | Světlá kronika — rozložení, typografie a obsah varianty 01 v barvách varianty 03. Bílá a světle šedé pásy, hluboká klubová zeleň, tenisově žlutá; stříbro z loga jen na tmavě zelených blocích. |

Barevnost všech variant vychází z klubového loga: tmavě zelená cedule, kartáčované stříbro
a žlutozelený tenisový míček.

### Varianta 04 — proč vznikla
Klub chce světlý web v klubových barvách. Varianta 04 je proto Kronika (01) beze změny
rozložení a funkcí — časová osa, zeď odchovanců, medailon 1953, přihláška, ceník — přebarvená
do palety Extraligy (03):

- plochy bílé a světle šedé `#F2F4F1`, text `#101713`
- hluboká zeleň `#14301F` na horní liště, přihlášce, patičce a klíčových blocích (Ex Pilsen,
  kempy, velké zápisy časové osy, zázemí areálu) — tam zůstává stříbrný kov letopočtů z loga
- klubová zeleň `#1E6B45` na tlačítkách, zvýrazněných slovech a letopočtech na bílé
- tenisově žlutá `#C8DE4A` jako jiskra: podtržení v hero, odlesk na medailonu 1953, body osy,
  linky u nadpisů sekcí

Navíc oproti ostatním variantám:

- **Aktuality s fotkami** z webu a letáků klubu (`assets/aktuality/`). V klidu jsou černobílé,
  barva naskočí při najetí myší, při procházení klávesnicí a na mobilu u karty uprostřed
  obrazovky. Přes fotky nejde žádný text. Seznam článků odpovídá webu klubu k září 2026 —
  přibyl „Ceník pro zimní sezónu 2026/2027“, letní ceník 2026 klub z webu stáhl.
- **Plánek areálu** ze skutečných dat OpenStreetMap.

## Co je ve všech variantách nového

### Přihláška do klubu
Třídílný registrační formulář: výběr typu členství s cenami z ceníku → osobní údaje
(u dětských kategorií se přidá blok pro zákonného zástupce) → rekapitulace a souhlasy.
Zatím jde o návrh chování — formulář se nikam neodesílá.

### Sekce trenéři
Karty vedení akademie a klubu. Jménem jsou uvedeni vedoucí akademie Jana Hollerová
a Mgr. Jiří Kovářík a výkonný výbor. Ostatní trenéry akademie doplníme podle aktuálního
seznamu klubu.

### Články klubu (Aktuality)
Sekce `#aktuality` s hlavním článkem, mřížkou karet a funkčním filtrem podle kategorií
(Vše · Klub · Akademie · Kempy · Ceník · Kurzy). Obsahuje osm skutečných článků, které klub
zveřejnil — od členské schůze a ceníků přes nábory do akademie až po kurzy pro
nejmenší. Odkaz „Aktuality" je první položkou hlavní navigace.

### Přehledný ceník
Kulaté přepínače mezi ceníky, sekce s barevnou hlavičkou
navazující přímo na tabulku, vedlejší sloupce s časem a podmínkou, cena vpravo tučně.
Na mobilu se tabulka rozpadne na bloky. Obsahuje zimní sezónu 2025/26 po časových pásmech
včetně členských cen, letní antuku a roční členské příspěvky.

## Obsah

Převzatý z webu klubu a z veřejných zdrojů:

- historie od roku 1953 — DSO Slavia, I. liga 1966, 3. místo 1968/69, extraliga od 1974
- turnaj **Ex Pilsen** (od 1971, juniorský okruh ITF) — Hewitt, Šarapovová (vítězka 2001)
- odchovankyně — Barbora Strýcová, Andrea Sestini Hlaváčková, Eva Birnerová
- akademie — Nadační fond Plzeňské regionální tenisové akademie (2017), tři programy, čísla 2024
- letní kempy 2026, družstva, areál (17 antukových dvorců, 6 krytých, bazén, fyzioterapie)

## Logo a rezervace

- Logo klubu je v `assets/logo-tk-slavia-trim.png` (ořez pro hlavičku a patičku). Na tmavých
  plochách leží na světlé podložce, protože po odmazání pozadí kolem míčku zůstává jemný závoj po stínu.
- Favicony `favicon-32/64/180.png` jsou zapojené ve všech variantách.
- Rezervace kurtů vedou na **https://www.rogeronline.cz/v2/?klub=103**.

## Technicky

- Statické HTML, jeden soubor na variantu, žádný build.
- Fonty z Google Fonts, jinak vše self-contained.
- Vizuály kreslené v CSS a inline SVG; ve variantě 04 navíc fotky klubu v Aktualitách.
- Plánek ve variantě 04 je vektorová ilustrace ze skutečných dat OpenStreetMap (areál TJ Slavia VŠ,
  jednotlivé kurty, haly, Borský park, ulice, stromy) v barvách klubu. Licence ODbL — pod plánkem
  je uvedeno „Mapová data © přispěvatelé OpenStreetMap“, to tam musí zůstat.
- Odladěno pro desktop i mobil (od 360 px). Stránky mají `noindex` — jde o návrh, ne o oficiální web.

## Co doplnit před nasazením

- [ ] **Fotografie** areálu, trenérů, akademie a historické snímky z archivu klubu (ve 04 jsou zatím fotky z webu a letáků klubu).
- [ ] **Trenérský tým** — doplnit ostatní trenéry akademie podle aktuálního seznamu klubu.
- [ ] **Přihláška** — napojit na odesílání (e-mail nebo databáze), potvrzovací e-mail, text GDPR souhlasu.
- [ ] **Rezervace kurtů** — dnes odkaz do systému Roger; jde vložit i přímo do stránky.
- [ ] **Ceník a telefon** — přepsat na ceník zima 2026/27 (klub ho vydal 18. 9. 2026), potvrdit příspěvky, doplnit hlavní telefon na klub (současný web ho neuvádí).
