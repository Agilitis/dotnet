## ASP.NET Core Web API
* Szerver oldali autentikáció **\[7-15\]**
  * token alapú, ASP.NET Core Identity + IdentityServer4 middleware-rel, interaktív flow **12**
* szerver oldali hozzáférés-szabályozás, az előbbi authentikációra építve  **\[2-5\]**
    * szerepkör alapú hozzáférés-szabályozás **2**
    * claim alapú hozzáférés-szabályozás **5**
    
* hosztolás külső szolgáltatónál **\[5-7\]**
  * Azure (ingyenes App Services - WebApp szolgáltatás) **7**
* Publikálás docker konténerbe és futtatás konténerből **\[7\]**

## Entity Framework Core

* újrapróbálkozás beállítása tranziens adatbázishibák (pl. connection timeout) ellen **\[2\]**
* adatbetöltés (seeding) migráció segítségével (`HasData`) **\[3\]**
* `DbContext` health check végpont publikálása a *Microsoft.Extensions.Diagnostics.HealthChecks.EntityFrameworkCore* NuGet csomag használatával **\[3\]**
  
## .NET Core részfunkciók alkalmazása
* kifejezésfa (ExpressionTree) értelmezése és manipulálása **\[5-20\]**
    * pl. szűrés dinamikusan, paraméterből érkező property neve alapján (pl. `o => o.Prop == propNev`) **5**
    * pl. keresés kapcsolódó kollekcióban dinamikusan (pl. `o => o.Coll.Any(e => e.Prop == propNev)`) **10**

* unit tesztek készítése  **\[7-14\]**
  * minimum 10 függvényhez **7**
  * a unit tesztekben a mock objektumok injektálása **+3**
  * EF Core memória-adatbázis vagy sqlite (vagy in-memory sqlite) használata teszteléshez **+4**

* diagnosztika beépített vagy külső komponens segítségével **\[5-9\]**
  * legalább két célba, amiből legalább egy perzisztens (pl. fájl vagy adatbázis vagy külső szolgáltatás) **5**
  * struktúrált naplózás (structured logging) **+2**

## Kiegészítő, kapcsolódó technológiák alkalmazása

* külső osztálykönyvtár használata (a külső komponensért további pontszám nem adható) szerver oldalon. Nem számít ide a projekt generálásakor bekerülő (pl. JSON.NET), illetve a Microsoft által készített, az alaptechnológiák függőségeit jelentő NuGet csomagok **\[7\]**
