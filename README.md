# 🍕 Pizza deník

Jednoduchý zápisník pokusů s pizza těstem. Běží celý v prohlížeči, nepotřebuje Claude ani žádný server.

U každého pokusu se zapisuje: název, datum, druh mouky, hydratace, sůl, droždí (+ typ), olej,
preferment (typ, % mouky, hodiny, teplota), libovolný počet fází zrání (hodiny + teplota),
počet a váha bochánků (z toho se dopočítá gramáž surovin), pec, hodnocení a poznámky.

## Spuštění

**Nejrychleji:** otevři `index.html` v prohlížeči. Data se ukládají v tom prohlížeči.

**Na PC i mobilu (doporučeno) přes GitHub Pages, zdarma:**
1. Na GitHubu vytvoř nový repozitář, třeba `pizza-denik` (může být veřejný, data v něm nejsou).
2. Nahraj do něj všechny soubory z této složky (*Add file → Upload files*).
3. *Settings → Pages → Branch: `main`, složka `/ (root)` → Save*.
4. Za chvíli bude aplikace na `https://<tvuj-ucet>.github.io/pizza-denik/`.
5. Na mobilu adresu otevři a dej *Sdílet → Přidat na plochu* (iPhone) nebo *⋮ → Přidat na plochu* (Android).
   Aplikace pak funguje i offline.

## Synchronizace PC ↔ mobil

1. Vytvoř token: <https://github.com/settings/tokens/new?scopes=gist&description=Pizza%20den%C3%ADk>
   (Tokens classic, zaškrtni jen **gist**).
2. V aplikaci ⚙ → vlož token → *Uložit a synchronizovat*. Udělej totéž na druhém zařízení se stejným tokenem.

Data se ukládají do tajného gistu `pizza-denik.json` ve tvém GitHub účtu. Synchronizace proběhne
automaticky při otevření aplikace a po každém uložení, ručně tlačítkem ⟳. Když stejný pokus upravíš
na dvou zařízeních, zůstane novější verze. Token je uložený jen v prohlížeči daného zařízení.

## Záloha

⚙ → *Export JSON* (záloha, lze zpět importovat) nebo *Export CSV* (otevřeš v Excelu).
