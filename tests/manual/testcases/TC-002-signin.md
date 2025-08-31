## TC-002: Kasutaja sisselogimine
**Kriitilisus:** High  
**Kategooria:** Authentication  
**Eeltingimused:** Kasutaja on registreeritud e-postiga `test@example.com` ja parooliga `Test123!`  

| Samm | Tegevus | Oodatav tulemus |
|------|---------|-----------------|
| 1    | Ava rakenduse avaleht | Avaleht laeb edukalt |
| 2    | Kliki "Sign In" nupul | Sisselogimisleht avaneb |
| 3    | Sisesta e-post `test@example.com` | E-post väli täidetakse |
| 4    | Sisesta parool `Test123!` | Parool väli täidetakse |
| 5    | Kliki "Login" nupul | Kasutaja logitakse sisse, suunatakse dashboard'ile |
| 6    | Kontrolli kasutaja nime kuvamist | Kasutajanimi kuvatakse navigatsioonis |

**Märkused:** Vale parooliga sisselogimine peaks näitama vea teadet.
