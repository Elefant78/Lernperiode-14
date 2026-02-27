# Lernperiode-14
Die Dokumentare Seite unseres 21-Gambling Spiels, hier befindet sich das README und die dazu gehörigen Arbeitspakete.

## 21-Gambling
Die ultimative Echtzeit-Blackjack-Erfahrung für dich und deine Freunde.

__21-Gambling__ ist eine moderne Web-Applikation, die das klassische Casino-Feeling direkt in den Browser bringt. Unser Fokus liegt auf einem nahtlosen __Multiplayer-Erlebnis:__ Erstelle eine Lobby, teile den Link und tritt gemeinsam mit bis zu 3 weiteren Spielern gegen die Bank (CPU) an. Anstatt gegen anonyme Gegner zu spielen, ermöglicht unsere 21-Gambling-Website private Spielrunden durch ein einfaches Einladungs-System.

## Kern-Features
- __Instant Lobbies:__ Erstelle einen Spielraum und verschicke den Einladungs-Link (wie bei skribbl.io).

- __Echtzeit-Action:__ Jede gezogene Karte und jeder Einsatz wird dank WebSockets sofort für alle Spieler synchronisiert.

- __Multiplayer vs. Bank:__ Bis zu 4 Spieler können gleichzeitig am Tisch Platz nehmen und versuchen, den Dealer zu schlagen.

- __Smart Dealer Logic:__ Eine automatisierte Bank, die strikt nach den offiziellen Blackjack-Regeln agiert (Stand bei 17).

- __Responsive Design:__ Optimiert für flüssiges Gameplay und intuitive Bedienung.



## Tech Stack
Für maximale Performance und eine geringe Latenz setzen wir auf folgende Technologien:

- Frontend: React.js mit Tailwind CSS für ein dynamisches und hochperformantes User Interface.

- Backend: Node.js & Express als zentrales Nervenzentrum für die Spiellogik.

- Echtzeit-Kommunikation: Socket.io für die bidirektionale Synchronisation zwischen Server und allen Clients.

- Hosting: Bereitgestellt auf Microsoft Azure (App Services), inklusive aktivierter WebSockets für stabiles Multiplayer-Gaming.



## Entwicklung & Workflow
Unser Team arbeitet nach strengen agilen Prinzipien, um in 7 Wochen ein fertiges Produkt zu liefern:

- Git-Strategie: Modularer Aufbau durch Feature-Branches und konsequente Code-Reviews.

- Arbeitspakete: Jede Sitzung wird in 12 spezifische Tasks unterteilt, um einen stetigen Fortschritt und saubere Commits zu garantieren.

- Security: Die Spiellogik (Kartenmischen, Werteberechnung) findet ausschließlich auf dem Server statt, um Manipulationen zu verhindern.
&nbsp;
---

&nbsp;

# Die Spielregeln

### Ziel
- Mehr Punkte als der Dealer erreichen, ohne die **21** zu überschreiten.

### Kartenwerte/Set
- **2 bis 10** = Nennwert  
- **J, Q, K** = 10 Punkte  
- **Ass** = 1 oder 11 Punkte (flexibel)
- **Sets** die anzahl sets ist von 1-6 frei wählbar. 

### Der „Blackjack“
- Ein **Ass** und eine **10er-Karte** direkt beim ersten Geben  
- Zahlt meist das **3:2**

### Aktionen
- **Hit**: Weitere Karte ziehen  
- **Stand**: Keine weitere Karte ziehen  
- **Double Down**: Einsatz verdoppeln, genau eine weitere Karte erhalten  
- **Split**: Bei zwei gleichen Karten das Blatt teilen (erfordert zwei separate Einsätze)  


### Dealer-Regel
- Der Dealer muss ziehen, bis er mindestens **17 Punkte** hat  
- Beachtet wird die **Soft-17-Regel**

### Turns
- **Start** Der Dealer verteilt die offnen Karten von links nach rechts und beendet den Spielzug mit der Upcard (offnen Karte)
- **Second** Der Dealer verteilt die Karten wieder in der reihen folge, die zweite Karte des Dealers ist verdeckt (Hole Card)
- **Player Action** Nach dem intital Deal, handeln alle Spieler nach ihren wwünschen und in der Reihenfolge. Der Dealer handelt erst am Schluss.
- **Dealer's Turn** Erstens deckt der Dealer seine verdeckte Karte auf, der Dealer zieht weitere Karten, bis er mindestens 17 Punkte erreicht hat (festgelegte Regel).

### Win
- bei einen Gewinn der Spieler gewinnen sie das 1 Fache ihres Einsatzes, dass heisst bei einem Einsatz von 10 gewinnt er Spieler 10, also bekommt er 20 zurück insgesamt

&nbsp;

---

&nbsp;


## Projektverlauf

[Projekt-Ordner](https://github.com/Fynn8962/21)

&nbsp;



&nbsp;

## Arbeit 20.02.2026



### Tages Zusammenfassung         

__Fynn Huber__            
Heute haben wir als Team uns eine Projektidee ausgedacht und die dafür nötigen Techniken ausgewählt. Anschliessend habe ich das GitHub-Repo für den Code erstellt, auf welches mithilfe von Git der Code hochgeladen wird. Anschliessend habe ich die Projektstruktur für das Frontend erstellt und gepusht.

__Doruk Güler__             
Heute habe ich mich mit meinen Teamkollegen zusammengesetzt und zunächst ein Brainstorming durchgeführt, um verschiedene Ideen zu sammeln und zu strukturieren. Im Anschluss daran habe ich die Ordnerstruktur für das Backend erstellt und diese in das GitHub-Repository hochgeladen.

__Tim Tafolli__                   
Heute habe ich mich mit meinen Teamkameraden zusammengesetzt und erst einmal gebrainstormt, was für Ideen uns in den Sinn kommen. Das hat länger gebraucht als gedacht, weil wir zwei gute Ideen hatten und uns nicht richtig entscheiden konnten für eine. Ich habe mich auch dran gemacht, einen kleinen Text zu schreiben. Bei den Dritten habe ich erfahren können, worum es bei unserem Projekt geht. 


&nbsp;

## Arbeit 27.02.2026        

**Arbeitspakete** Tim Tafolli         
- [x] Blackjack spielregen defineiren
- [X] Generieren eines Kartendecks 52 karten (in Javascript)
- [ ] Logik für das Mischen der Karten (In JavaScript)
- [x]  Pitch planen / erstellen

**Arbeitspakete** Doruk Güler         
- [x] Grundlegendes Express server Setup (Hello World)
- [ ] Socket.io auf dem Server initialisieren
- [x] .gitignore für Node ersellen
- [x]  Pitch planen / erstellen

**Arbeitspakete** Fynn Huber         
- [x] React BSP Projekt aufräumen und eigene Filestruktur erstellen
- [x] Grundstruktur der Website erstellen (gerüst)
- [x] tailwind CSS installieren und Konfigurieren
- [x]  Pitch planen / erstellen

&nbsp;

**Tages Zusammenfassung**                 

__Fynn Huber__    
Heute habe ich das React-Projekt aufgeräumt und die Dateien hinzugefügt, welche in Zukunft benutzt werden. Danach habe ich angefangen mit dem Handhaben der Lobby und Spieler, da dies das Erste ist, was wir realisieren wollen, sodass sich eine Lobby mit mehreren Spielern erstellen lässt. Zusätzlich habe ich Tailwind im Projekt eingefügt für eine einfachere Handhabung des Stylings.

__Doruk Güler__
Heute habe ich das Backend das heisst die Express.js Dateien erstellt. Danach habe ich das Socket.io auf dem erstelltem Server initialisiert. Ebenfalls habe ich den ersten Lobbysysthem mit Socket.io implementiert so dass ein Lobby mit ID erstellt wird und man mit dieser ID dann denn room von freunden joinen kann.

__Tim Tafolli__
Heute habe ich, kurz an der Definition des Spiels festgehalten, damit jede Person weiss, wie Blackjack funktioniert und welche Features wir eingebaut haben. Im zweiten Teil habe ich mich an die Logik der Kartensätze und des Decks selber, also aller 52 Karten, gehalten. Hier war es wichtig, die Funktion so zu machen, dass der Spieler die Auswahl der Kartensätze treffen kann. Ich habe weiter an der Shuffle-Funktion gearbeitet. Ich habe mich mit Ki's darüber informiert, welcher Algorithmus sich eignet. Dabei bin ich auf den Fisher-Yates Shuffle gestossen. 	


&nbsp;

## Arbeit 06.03.2026        

**Arbeitspakete** Tim Tafolli         
- [ ] Logik für das Mischen der Karten (In JavaScript)


**Arbeitspakete** Doruk Güler   
- [ ] Individuelle Lobbys IDs erstellen      
- [ ] Lobby mit ID beitreten
- [ ] Lobbysysthem ans Frontend anpassen


**Arbeitspakete** Fynn Huber         
- [ ] Fertigstellung des Codes für das Handling der Lobby und Spieler. 
- [ ] Die Spielerliste anzeigen im Browser (welche spieler in der Lobby sind)
- [ ] Lobby einstellungen definieren (im Team besprechen) und diese Einstellungen in der ansichten einbinden
- [ ] Spiel Starten Button hinzufügen um das Spiel zu starten (Bereit Button für die anderen Teilnehmer)


&nbsp;

**Tages Zusammenfassung**          
