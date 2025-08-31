# Medium Clone Test Plan

**Versioon:** 1.0  
**Kuupäev:** 31.08.2025  
**Autorid:** Lembit Lindau  

## 1. Pealkiri, versioon, autorid

**Dokumendi nimi:** Medium Clone Test Plan  
**Versioon:** 1.0  
**Autorid:** Lembit Lindau  
**Kuupäev:** 31.08.2025  
**Projekt:** Medium Clone veebirakendus  

## 2. Dokumendi ajalugu ja heakskiidud

| Versioon | Kuupäev | Muudatused | Autor |
|----------|---------|------------|-------|
| 1.0 | 31.08.2025 | Algne testplaan | Lembit Lindau |

**Heakskiidud:**
- Testijuht: Lembit Lindau (31.08.2025)

## 3. Eesmärk ja ulatus

**Eesmärk:** Tagada Medium Clone veebirakenduse funktsionaalsuse, kasutajamugavuse ja jõudluse kvaliteet enne tootmiskeskkonda juurutamist.

**Testede ulatus:**
- Kasutaja autentimine (sisselogimine, registreerimine)
- Artiklite loomine, redigeerimine ja kustutamine
- Artiklite lugemine ja kommenteerimine
- Kasutajaprofiili haldamine
- Põhilised UI/UX elemendid

**Välja jäetud:**
- Jõudlustestid suure koormuse all
- Turvatestid (penetratsiooni testid)
- Mobiilirakenduse testid

## 4. Viited ja alusdokumendid

- Frontend repo: https://github.com/lembitlindau/-Medium-clone-frontend
- Backend repo: https://github.com/lembitlindau/Medium-clone-API
- Medium.com originaal funktsionaalsus (referents)

## 5. Testitavad üksused

**Frontend komponendid:**
- Kasutajaliides (React komponendid)
- Navigatsioon
- Vormid ja validatsioon

**Backend API:**
- Autentimise endpointid
- Artiklite CRUD operatsioonid
- Kasutajate haldus
- Andmebaasi integratsioon

## 6. Testitavad ja mittetestitavad omadused

**Testitavad funktsionaalsused:**
- Kasutaja registreerimine ja sisselogimine
- Artiklite loomine ja publitseerimine
- Artiklite lugemine ja otsing
- Kommentaaride süsteem
- Kasutajaprofiili haldus

**Mittetestitavad:**
- Kolmandate osapoolte integratsioonid
- Backup ja taastamise protseduurid
- Skaleeritavus üle 1000 kasutaja

## 7. Testimise lähenemine

**Testimise tüübid:**
- Funktsionaalne testimine (käsitsi)
- UI/UX testimine
- API testimine
- Integratsioonitestid
- Smoke testid

**Tööriistad:**
- Käsitsi testimine: brauser (Chrome, Firefox)
- API testimine: Postman/curl
- Automaattestid: Cypress (tulevikus)

## 8. Sisenemis-, väljumis- ja peatamiskriteeriumid

**Sisenemiskriteeriumid:**
- Kõik komponendid on arenduses valmis
- Test keskkond on seadistatud
- Testandmed on ettevalmistatud

**Väljumiskriteeriumid:**
- 95% testjuhtumitest on läbitud edukalt
- Kõik kriitilised vead on parandatud
- Performance vastab nõuetele

**Peatamiskriteeriumid:**
- Rohkem kui 5 kritilist viga
- Test keskkond ei ole kättesaadav > 24h
- Ajakavas olulised hilinemised

## 9. Ressursid ja rollid

**Testimeeskond:**
- Testijuht: Lembit Lindau
- Testiinsener: Lembit Lindau

**Keskkond:**
- Test server: lokaalne arenduskeskkond
- Andmebaas: PostgreSQL/MongoDB

## 10. Ajakava ja verstapostid

| Faas | Alguskuupäev | Lõppkuupäev | Vastutaja |
|------|--------------|-------------|-----------|
| Testplaani koostamine | 31.08.2025 | 02.09.2025 | Lembit Lindau |
| Testjuhtumite koostamine | 02.09.2025 | 05.09.2025 | Lembit Lindau |
| Testimine | 05.09.2025 | 15.09.2025 | Lembit Lindau |
| Raportite koostamine | 15.09.2025 | 17.09.2025 | Lembit Lindau |

## 11. Keskkond ja infrastruktuur

**Test keskkond:**
- Frontend: localhost:3000
- Backend API: localhost:8000
- Andmebaas: lokaalne PostgreSQL/MongoDB
- Operatsioonisüsteem: Linux
- Brauserid: Chrome 126+, Firefox 115+

## 12. Testide disaini viited

- Käsitsi testid: `/tests/manual/testcases/`
- Automaattestid: `/tests/automation/` (tulevikus)
- Test template: `/tests/manual/testcases/testcase-template.md`

## 13. Riskid ja leevendused

| Risk | Tõenäosus | Mõju | Leevendamine |
|------|-----------|------|-------------|
| Test keskkonna kättesaamatus | Madal | Kõrge | Backup keskkond |
| Testijate puudus | Madal | Keskmine | Cross-training |
| Ajakavas hilinemised | Keskmine | Keskmine | Prioritiseerimine |

## 14. Luba- ja auditeerimisnõuded

**N/A** - Projekt ei nõua spetsiifilisi luba või auditeerimise nõudeid käesolevas faasis.

## 15. Testi töövoo protseduurid

**Defekti elutsükkel:**
1. Avastamine → GitHub Issue
2. Kategoriseerimine (kriitilisus)
3. Määramine arendajale
4. Parandamine
5. Uuesti testimine
6. Sulgemine

## 16. Mõõdikud ja raportid

**KPI-d:**
- Test katvus: 100% kriitiliste funktsionaalsuste
- Defektide arv komponendi kohta
- Testimise edenemise protsent

**Raportite sagedus:**
- Iganädalased progress raportid
- Lõplik test-run raport

## 17. Lõpuleviimise kriteerium ja hooldus

**Lõpuleviimise kriteeriumid:**
- Kõik planeeritud testjuhtumid on täidetud
- Kriitilised vead on parandatud
- Test raport on kinnitatud

**Hooldus:**
- Testplaani uuendamine uute nõuete lisandumisel
- Test juhtumite täiendamine

## 18. Testjuhtumite loetelu

Testjuhtumid asuvad kaustas: `/tests/manual/testcases/`

**Planeeritud testjuhtumid:**
- TC-001: Kasutaja registreerimine
- TC-002: Kasutaja sisselogimine
- TC-003: Artikli loomine
- TC-004: Artikli redigeerimine
- TC-005: Artikli kustutamine
- TC-006: Artikli lugemine
- TC-007: Kommentaari lisamine
- TC-008: Kasutajaprofiili vaatamine
- TC-009: Kasutajaprofiili redigeerimine
- TC-010: Väljalogimine
- TC-011: Artiklite otsing
- TC-012: Artiklite filtreerimine

## 19. Test-run'i raportid

Test-run'i raportid asuvad kaustas: `/reports/`

**Planeeritud raportid:**
- `testrun_2025-09-10.md` - Esimene test-run
- `testrun_2025-09-15.md` - Lõplik test-run
