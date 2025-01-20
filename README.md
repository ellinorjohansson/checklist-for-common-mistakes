# Vanliga misstag 🔍

> [!NOTE]  
> Lista hämtad från skolan och sparad för framtida projekt, som en reminder till mig själv.

---

## HTML / CSS 👋

### Allmänna riktlinjer
- **Alt-texter på bilder:** Kom ihåg att alltid sätta alt-texter på bilder för tillgänglighet och SEO.
- **Sätt inte ID-attribut utan anledning:** Använd ID endast om det är nödvändigt.
- **Använd gemener för HTML-taggar.**
- **Undvik `<br>` i HTML:** Använd istället CSS för radbrytningar. Använd `<br>` endast för specifika behov.
- **Använd `<input>` inom `<label>`:** Det underlättar och du slipper använda `for` och `id`.
- **Telefonnummer:** Skriv alltid telefonnummer med landskod för att underlätta uppringning via mobil.

### Bildhantering
- **Bildens bredd och höjd:** Sätt alltid bredd och höjd för att undvika att sidan hoppar vid inladdning.
  - Exempel: `<img src="image.jpg" width="640" height="480" />`
- **Alt-text:** ALLTID en alt-text för alla bilder.
- **Optimera bildladdning:** Använd `loading="lazy"` för att optimera laddningen av bilder.
- **Bildnamn:** Använd beskrivande bildnamn utan specialtecken (å, ä, ö, etc.) och utan mellanslag (använd t.ex. `_` istället).

### Formulär
- **Byt ut `<button>` mot `<input type="submit">`** för att skicka formulär och `<input type="reset">` för att nollställa formulär.
- **Formatering:** Tänk på konsekvent formatering (mellanslag, radbrytningar, etc.).
- **Enheter:** Sätt aldrig en enhet efter ett värde om värdet är noll.

### CSS Tips
- **Citattecken för URL:** Sätt alltid citattecken runt URL:er i CSS. Exempel: `'hej/url.avif'`.
- **Versaler:** Fixa versaler i CSS, undvik att skriva versaler i HTML.
- **Formatering av kod:** Tänk på korrekt indentering för läsbarhet.
- **Import av fonter:** Importera inte fonter i CSS; använd istället en extern fil för detta. Glöm heller inte backup-font!
- **Sätt aldrig `px` på font-storlek:** Använd `rem` eller `em` istället.

### Tillgänglighet
- **Menyknapp:** Sätt alltid ett `aria-label` på menyknappen för att göra den tillgänglig för assistiva enheter om den är tom eller otydlig.
- **Tillgänglighetsgranskning:** Tänk alltid på tillgängligheten när du utvecklar.

### SEO
- **Testa sidan utan CSS:** Simulera hur sidan ser ut utan CSS för att säkerställa att innehållet är användbart även utan styling.
- **Sökmotoroptimering:** Använd rätt HTML-taggar och bildnamn för bättre SEO.

---

## JavaScript / TypeScript 🦄

### Allmänna riktlinjer
- **Namngivning:** Följ en konsekvent namngivning för både klasser och funktioner. Undvik att blanda `camelCase` och `kebab-case`.
- **Aria labels:** Kom ihåg att lägga till `aria-labels` för att stödja tillgängligheten.
- **Datumhantering:** Se till att datum uppdateras korrekt, särskilt om användaren lämnar sidan öppen under lång tid.

### Objekt och datatyper
- **Rätt datatyp:** När du skapar objekt, tänk på att använda rätt datatyp för att underlätta framtida ändringar.

### Script
- **Placering av script:** Sätt alltid `<script>`-taggen precis innan den avslutande `</body>`-taggen för att inte blockera sidans inladdning. Använd `defer` om du inte kan göra det.
- **Anonyma funktioner:** Undvik att använda anonyma funktioner för att skapa bättre läsbarhet och underhåll.
- **Init-funktion:** Skapa en `init`-funktion för att gruppera funktioner som ska köras när sidan laddas, istället för DOM.

---

## Övrigt
- **Validering:** Validera alltid både din HTML och CSS för att säkerställa att de följer standarder. Gör även Lighthouse analys.
- **Använd `.gitignore`:** Lägg till `.DS_Store` i `.gitignore` för att undvika att denna fil checkas in.
