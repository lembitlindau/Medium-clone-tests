# Medium Clone - Test Repository

See repositoorium sisaldab testplaani, testjuhtumeid ja test-run'i raporteid Medium Clone veebirakendusele.

## Projekt

- **Frontend:** https://github.com/lembitlindau/-Medium-clone-frontend
- **Backend:** https://github.com/lembitlindau/Medium-clone-API

## Repositooriumi struktuur

```
├── .github/workflows/
│   └── ci.yml                  # CI/CD workflow
├── tests/
│   ├── manual/
│   │   ├── testplan.md         # 19-jaotisega testplaan
│   │   └── testcases/          # 12 testjuhtumit
│   │       ├── testcase-template.md
│   │       ├── TC-001-registration.md
│   │       └── ...
│   └── automation/             # (tulevikus automaattestid)
├── reports/
│   └── testrun_2025-08-31.md   # Test-run raport
└── README.md
```

## Kiire ülevaade

**Testplaan:** `/tests/manual/testplan.md`
- 19 jaotist IEEE 829 standardile vastavalt
- Määratleb testimise strateegia ja protsessi
- Sisaldab riske, ressursse ja ajakavasid

**Testjuhtumid:** `/tests/manual/testcases/`
- 12 testjuhtumit (60% plaanitud 20-st)
- Katab põhilised funktsionaalsused:
  - Autentimine (registreerimine, sisselogimine)
  - Artiklite CRUD operatsioonid
  - Kasutajate haldus
  - Otsing ja filtreerimine

**Test-run raportid:** `/reports/`
- Esimene test-run: 67% edukus (8/12 PASS)
- 2 viga avastatud ja dokumenteeritud
- 2 funktsionaalsust blokeeritud (ei ole implementeeritud)

## Käivitamine

1. **Klooni repositoorium:**
   ```bash
   git clone https://github.com/lembitlindau/Medium-clone-tests.git
   cd Medium-clone-tests
   ```

2. **Vaata testplaani:**
   ```bash
   cat tests/manual/testplan.md
   ```

3. **Käivita testjuhtumid:**
   - Käsitsi testimine: järgi samme testjuhtumites
   - CI/CD: push'i muudatused, GitHub Actions käivitab valideerimise


## Kontakt

**Autor:** Lembit Lindau  
**Kuupäev:** 31.08.2025