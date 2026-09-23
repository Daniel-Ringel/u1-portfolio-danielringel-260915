# Daniel Ringel - Portfolio


A portfolio site built from Pawan's Figma design.

**Live site:** https://daniel-ringel.github.io/u1-portfolio-danielringel-260915/index.html

## Built with:
- HTML
- CSS (Flexbox and Grid)
- Google Fonts (Poppins)

## Reflektion

### Från skiss till kod

Jag började med att planera hur själva sidans skelett skulle se ut och hur det skulle vara enklare att kontrollera bakgrunden.

Min plan var i sig att börja med att göra en HTML- och en övrig "base.css" -fil som styr allt över varje sida.

Så det skulle vara enklare att kontrollera än att gå in en och en.

Även med navigeringen och länkarna. Det enda som blev själv var då main elementet som är i sig då content som man ser i sidan.

Det svåraste utifrån kodningen och vad jag försökte göra i skissen var säkert själva kodningen i sig, när man redan har börjat någonstans och ska behöva justera någonting. Det blir svårt senare att behöva byta, kanske en kod och vilja lägga den i en annan. Beroende på vilket t.ex. HTML-elementtags ska användas och göras så rätt som möjligt.

Hur jag löste ut problemet var att jag fick skriva om några få delar (lägga till klasser) och se till att det sitter rätt, byta också element taggar när det behövdes om det fanns ett bättre alternativ som jag kom fram till.

### Semantik

Alla sidor innehåller header, main och footer. I nav använder jag ul och li eftersom länkarna till de fem sidorna är en lista.  Samma navigering är planerad och ska finnas i alla HTML-filer, så att det är enkelt att ta sig runt på sidan.

På Projects.html är varje projektkort en article. Jag valde detta eftersom varje projekt ska kunna stå för sig själv och det blir enkelt att lägga till fler projekt framöver.

På Tech Stack bytte jag en span till en section. Jag fick feedback om att det skulle bli fel i validatorn, eftersom en span bara får innehålla text, medan en section är gjord för att gruppera en del av sidan med en egen rubrik.

Menyknappen är en button eftersom det är tänkt att den ska användas med JavaScript i nästa uppgift som kommer, för att visa och dölja menyn på mobilen. En button fungerar dessutom med tangentbordet direkt.

Jag använde en div för photo-frame eftersom inget annat element fanns som kändes relevant för fotoram. Den är bara till för utseendet, den gradientfärgade ringen runt bilden, och är inget eget innehåll.

I projektkorten använde jag också div för project-body och project-links. De är bara till för att samla texten och länkarna så att det går att styla dem med padding och flexbox, och det fanns inget annat element som kändes mer rätt där.

### Layout

Jag använde flexbox väldigt mycket i header/nav och main. 

Anledningen till varför jag kom till detta beslut var för att det skulle vara enklare att styra och se till att t.ex. footer sitter alltid nere.

Samma med logon av sidan, att det sitter längst mot vänster i header. 

Grid använde jag mer på About, Projects och Tech Stack, för att kunna ordna upp delarna rätt. Jag kände att det passade bäst där, eftersom jag enkelt kunde lägga till och styra utseendet, medan flexbox är mer för saker i en linje.

Bästa exemplet med flexbox är att jag kan se det som en rak elev kö inför en lunch.

Flexbox är eleverna som är då i kö högst upp, ingången av  själva lunchsalen. Medans borden och stolarna är grid'en.

Jag skrev CSS:en för mobilen först, och lade sedan till en media query med min-width: 600px för desktop. Jag valde 600px eftersom skissens mobillayout är 600px bred, så allt över det får desktoplayouten.

### Tillgänglighet

För att fler ska kunna använda sidan har jag använt alt-text där det behövdes, så att en skärmläsare kan läsa upp vad bilden visar, och tom alt="" när det handlade om dekoration. Aria-label använde jag för ikonlänkarna, eftersom de inte har någon text. Jag gjorde också färgerna mörkare så att texten blir lättare att läsa.

Jag testade sidan med validatorn, som visade 0 fel, och i Firefox och Safari på min iPhone.

Det som återstår är gradienttexten i logon och footern, som har lite för låg kontrast, och menyknappen som inte gör något än.

### Användarbarhet

I Pawans design känner jag igen principen konsekvens, eftersom header, navigering och footer ser likadana ut på alla sidor. Då vet användaren alltid var man hittar saker. Jag ser också visuell hierarki, de stora rubrikerna syns först, och mindre viktigt text är grå.

Det jag hade gjort lite annorlunda är framsidan och Contact-sidan. På framsidan kunde man ha lagt till exempel ett "senaste projekt" och ändrat strukturen i main, så att det ser finare ut och passar kommande idéer.

Contact känns lite för tom, med bara ett kort meddelande och en mejladress. Jag skulle lägga till ett formulär där besökaren kan skriva sin egen mejladress och ett meddelande, så att jag kan höra av mig tillbaka.

### Styrkor och brister

En styrka är att strukturen gör det enkelt att skapa nya sidor. Det enda man behöver göra för att fortsätta och skapa en ny sida är att duplicera eller kopiera kodens html till en ny sida. Ta bort bara innehållet i main och skapa en ny CSS-fil som man kopplar upp på nytt inom link taggarna. 

Om jag hade mer tid så skulle jag då sitta mer med att försöka strukturera CSS koden finare.

### AI-verktyg

Jag använde AI (Claude) för att få feedback på koden. Jag använde AI även för att förstå saker som dark mode och GitHub Pages, och Git-kommandon.

När det kom till att fixa upp saker som about.css med display: grid så använde jag AI där för att förstå upplägget med hur man gjorde allt och skapade en ordentlig grid.

Det som jag ändrade av det som genererades var mest antalet kolumner och hur det skrevs upp. (grid-template-columns) För att få det rätta antalet och att det skulle sitta rätt, några gånger föreslog den värden av width men det använde jag inte och skrev själv. Så att jag följde skissen så nära som möjligt.

