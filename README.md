# codebuddy
App som ska hjälpa elever lära sig python

<h2>1. Vision</h2>
CodeBud är en interaktiv webbapplikation utformad för att hjälpa nybörjare att lära sig grundläggande Python-programmering genom korta, interaktiva kodövningar och omedelbar feedback. Målet är att göra tröskeln till textbaserad programmering så låg som möjligt för gymnasieelever.

<h2>2. MVP (Minimum viable product</h2>
För att nå vår MVP i den första sprintcykeln ska applikationen innehålla följande kärnfunktioner:

<h3>Kärnfunktionalitet (Must-Have)</h3>
Övningslista: En vy där användaren kan se och välja mellan minst 5 grundläggande Python-övningar.
- Kodeditor: En enkel vy i webbläsaren där användaren kan skriva och redigera sin kod.
- Kodexekvering: Möjlighet att köra koden och se resultatet (output) i en konsol direkt på skärmen.
- Facit/Test: En knapp för att kontrollera om lösningen uppfyller övningens krav.

<h3>Avgränsningar (Out of Scope för MVP)</h3>
Inkluderas INTE i MVP, sparats till framtida releaser:

Användarkonton och inloggning (alla framsteg sparas enbart lokalt i webbläsaren).
Avancerad kodkomplettering (Auto-complete / Copilot-funktioner).
Flera programmeringsspråk (enbart Python i fas 1).

<h1>3. Målgrupp & Användarroller</h1>

Elev (Slutanvändare): Vill ha korta, tydliga instruktioner, kunna skriva kod direkt i webbläsaren utan installationer och få snabb feedback om koden är rätt eller fel.
Lärare (Administratör - Framtida roll): Vill kunna lägga till egna övningar och följa elevernas framsteg.

<h1>4. Teknisk Stack</h1>
Frontend: HTML5, CSS3 (Tailwind CSS), JavaScript (Vanilla eller React/Vite)
Kodmotor/Exekvering: Pyodide (Python körs direkt i webbläsaren via WebAssembly utan krav på backend)
Hosting/Deployment: GitHub Pages / Vercel

<h1>5. Arbetssätt & Git-strategi</h1>
Branch-struktur
main: Innehåller enbart stabil och testad kod. Direct commits till main är förbjudna.
feature/[kort-namn]: Skapas för varje ny funktion (t.ex. feature/code-editor eller feature/exercise-list).
Definition of Done (DoD)
En GitHub Issue / Task anses vara Done och klar att stängas när:

Koden uppfyller acceptanskraven för uppgiften.
Koden är testad och körs utan fel i lokal miljö.
En Pull Request (PR) har skapats mot main.
Minst en annan teammedlem har granskat och godkänt koden (Code Review).
Koden har mergats till main.
