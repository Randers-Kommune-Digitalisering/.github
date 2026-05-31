## Privacy by Design i Randers Kommune – Digitalisering
Dette dokument beskriver hvordan vi i Digitalisering i Randers Kommune inkorporerer Privacy by Design for at sikre, at databeskyttelse altid er en integreret del af vores arbejde med udvikling af nye applikationer og automatiseringsløsninger. Nedenfor beskrives, hvordan vi efterlever de syv grundlæggende principper i praksis.

### 1. Proaktivitet og risikostyring
Vi tager hensyn til databeskyttelse tidligt i vores projektforløb. Allerede i analysefasen vurderer vi, hvilke data der skal behandles, og om der kræves særlige tiltag for at beskytte dem. Vi undersøger de systemer, hvorfra data skal udtrækkes, og sikrer, at adgangen begrænses mest muligt – systembrugere får kun adgang til det data, der er nødvendigt for løsningen der udvikles.
Vi anvender en generel risikovurdering for behandling af følsomme data i vores produktionsmiljø. For hver ny applikation eller databehandling udarbejdes et særskilt bilag, der dokumenterer de særlige risici og tiltag. Systemejer samt evt. DPO inddrages i analysefasen for at sikre forståelse for både data og de risici, der er forbundet med brugen.

### 2. Standardindstilling (Privacy by Default)
Vi arbejder ud fra princippet om dataminimering og sikrer, at behandling og opbevaring af data altid begrænses til et minimum. Vi sikrer at data først hentes og behandles ved behov, og opbevarer kun data i den grad som det er nødvendigt for løsningens funktionalitet. Vi undlader at indsamle unødvendige brugerdata og brugsstatistik, og sikrer, at data kun er tilgængelige i de kontekster, hvor de skal anvendes.
Vi logger kun nødvendige data for udviklingsbrug og undgår logning af personoplysninger. Hvor det er nødvendigt at opbevare persondata, sker det i krypterede PostgreSQL-databaser.

### 3. Privacy integreret i designet
Privacy er en indbygget del af vores design- og udviklingsproces. Vi benytter standardiserede skabeloner i nye projekter, som sikrer, at vi altid anvender velafprøvede frameworks, databaser og sikre metoder til håndtering af data. Når det er muligt, trækker vi data direkte fra kilden for at undgå datavask og tab af datakvalitet.
Vi genbruger services til datatræk på tværs af løsninger, men sikrer separate credentials for at opretholde dataminimering. Credentials og andre adgangsgivende oplysninger opbevares i Bitwarden, og udviklerne har ansvar for, at disse oplysninger håndteres sikkert. I de tilfælde hvor adgangsgivende oplysninger skal være tilgængelige i applikationskontekst, sikres disse som Sealed Secrets, således de opbevares krypteret på driftsmiljøet.
Applikationer åbnes kun for trafik, hvis de udstiller API’er eller brugerinterfaces, og altid med sikkerhedsforanstaltninger som OpenID/ADFS-integration, IP-restriktioner eller, i begrænsede tilfælde, basic authentication til enkle endpoints uden persondata.
Alle dataflows dokumenteres og visualiseres i flowcharts, så det fremgår tydeligt, hvilke typer data der behandles, og hvordan de flyder i løsningen. Beslutninger og fravalg i forhold til privacy dokumenteres i bilag til databehandleraftaler. Pseudonymisering eller anonymisering anvendes som udgangspunkt ved udstilling af data, medmindre det er nødvendigt at fremstille identificerbare data for at understøtte arbejdsgangen.

### 4. Fuld funktionalitet
Vi balancerer funktionalitet og databeskyttelse gennem tæt samarbejde med fagområderne. Systemejere og medarbejdere, der arbejder med data til dagligt, inddrages i vurderingen af, hvilke data og funktioner der er nødvendige for at understøtte en digitalisering af arbejdsgangen.
Brugervenlighed testes løbende inden idriftsættelse. Når løsninger har brugergrænseflader, inddrager vi slutbrugere i testfasen for at finde den rette balance mellem funktionalitet, brugervenlighed og databeskyttelse. 

### 5. Vugge-til-grav (livscyklus for data)
Vi gemmer kun data, når det er absolut nødvendigt, og kun i den periode, der er nødvendig for, at applikationen kan fungere. Vores testmiljøer indeholder aldrig produktionsdata og er adskilt fra driftssystemerne.
Staging- og produktionsmiljøer er sikret med ugentlig kontrol af bagvedliggende sikkerhed på både databaser og applikationslag udført af vores driftsleverandør. Data som opbevares i drift, er som udgangspunkt krypteret, og al kommunikation til og fra miljøerne er beskyttet med SSL. Interne systemer forbindes via VPN-tunneller. 

### 6. Synlighed og gennemsigtighed
Vi følger Randers Kommunes samlede politik for kommunikation om databeskyttelse. Det betyder, at information til borgere og medarbejdere sker efter de gældende kommunale retningslinjer og processer. Vi udarbejder ikke særskilte privatlivspolitikker for hver applikation, men henviser til den samlede kommunale politik.
Brugere kan altid henvende sig til kommunens databeskyttelsesrådgivere (DPO’er), hvis de har spørgsmål eller bekymringer vedrørende behandling af deres data.

### 7. Brugerorientering
Vi følger kommunens standarder for udformning af privatlivsmeddelelser og samtykkeerklæringer, så de er klare og forståelige. Vi sikrer vi, at løsningerne er så gennemsigtige som muligt, og orienterer brugere i de tilfælde hvor data opbevares. 
De løsninger som vi udvikler, ændrer som udgangspunkt ikke på, hvordan data behandles – de automatiserer blot eksisterende arbejdsgange. Eventuelle oplysninger om, hvordan data og rettigheder påvirkes, håndteres derfor på fagområdeniveau, hvor de manuelle arbejdsgange i forvejen er beskrevet.

