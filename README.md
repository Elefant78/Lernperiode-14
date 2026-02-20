# Lernperiode-14
Die Dokumentare Seite unseres 21-Gambling Spiels, hier befindet sich das README und die dazu gehörigen Arbeitspakete.

## 21-Gambling
Die ultimative Echtzeit-Blackjack-Erfahrung für dich und deine Freunde.

__21-Gambling__ ist eine moderne Web-Applikation, die das klassische Casino-Feeling direkt in den Browser bringt. Unser Fokus liegt auf einem nahtlosen __Multiplayer-Erlebnis:__ Erstelle eine Lobby, teile den Link und tritt gemeinsam mit bis zu 3 weiteren Spielern gegen die Bank (CPU) an. Anstatt gegen anonyme Gegner zu spielen, ermöglicht unsere 21-Gambling-Website private Spielrunden durch ein einfaches Einladungs-System.

## Kern-Features
- __Instant Lobbies:__ Erstelle einen Spielraum und verschicke den Einladungs-Link (wie bei skribbl.io).

__Echtzeit-Action:__ Jede gezogene Karte und jeder Einsatz wird dank WebSockets sofort für alle Spieler synchronisiert.

__Multiplayer vs. Bank:__ Bis zu 4 Spieler können gleichzeitig am Tisch Platz nehmen und versuchen, den Dealer zu schlagen.

__Smart Dealer Logic:__ Eine automatisierte Bank, die strikt nach den offiziellen Blackjack-Regeln agiert (Stand bei 17).

__Responsive Design:__ Optimiert für flüssiges Gameplay und intuitive Bedienung.

🛠 Tech Stack
Für maximale Performance und eine geringe Latenz setzen wir auf folgende Technologien:

Frontend: React.js mit Tailwind CSS für ein dynamisches und hochperformantes User Interface.

Backend: Node.js & Express als zentrales Nervenzentrum für die Spiellogik.

Echtzeit-Kommunikation: Socket.io für die bidirektionale Synchronisation zwischen Server und allen Clients.

Hosting: Bereitgestellt auf Microsoft Azure (App Services), inklusive aktivierter WebSockets für stabiles Multiplayer-Gaming.

🏗 Entwicklung & Workflow
Unser Team arbeitet nach strengen agilen Prinzipien, um in 7 Wochen ein fertiges Produkt zu liefern:

Git-Strategie: Modularer Aufbau durch Feature-Branches und konsequente Code-Reviews.

Arbeitspakete: Jede Sitzung wird in 12 spezifische Tasks unterteilt, um einen stetigen Fortschritt und saubere Commits zu garantieren.

Security: Die Spiellogik (Kartenmischen, Werteberechnung) findet ausschließlich auf dem Server statt, um Manipulationen zu verhindern.

📖 Kurzregeln
Ziel: Erreiche 21 Punkte oder bleibe näher dran als der Dealer, ohne die 21 zu überschreiten (Bust).

Ablauf: Jeder Spieler startet mit zwei Karten. Entscheide zwischen Hit (ziehen) oder Stand (halten).

Dealer-Regel: Die Bank zieht Karten, bis sie mindestens 17 Punkte erreicht hat.
