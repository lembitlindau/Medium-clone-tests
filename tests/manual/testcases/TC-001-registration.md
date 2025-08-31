## TC-001: Kasutaja registreerimine
**Kriitilisus:** High  
**Kategooria:** Authentication  
**Eeltingimused:** Kasutaja ei ole veel registreeritud süsteemis.  

| Samm | Tegevus | Oodatav tulemus |
|------|---------|-----------------|
| 1    | Ava rakenduse avaleht | Avaleht laeb edukalt |
| 2    | Kliki "Sign Up" nupul | Registreerimisleht avaneb |
| 3    | Sisesta e-post `test@example.com` | E-post väli täidetakse |
| 4    | Sisesta kasutajanimi `testuser` | Kasutajanimi väli täidetakse |
| 5    | Sisesta parool `Test123!` | Parool väli täidetakse (peidetud) |
| 6    | Sisesta parool uuesti `Test123!` | Parooli kinnitus väli täidetakse |
| 7    | Kliki "Register" nupul | Kasutaja luuakse edukalt, suunatakse dashboard'ile |

**Märkused:** Parool peab sisaldama vähemalt 8 tähemärki, suuri ja väikesi tähti ning numbreid.
