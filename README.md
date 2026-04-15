# Trajectory Clustering

Dieses Projekt untersucht, wie sich verrauschte Wurfparabeln im 2D-Raum trennen, gruppieren und rekonstruieren lassen.

## Projektidee

Zwei ballistische Flugbahnen werden simuliert und mit Rauschen in x- und y-Richtung überlagert. Dadurch ist die Zuordnung der Messpunkte zu den ursprünglichen Wurfparabeln nicht mehr eindeutig.

Ziel ist es, die gemischten Messpunkte wieder in zwei Gruppen zu trennen und daraus die zugrunde liegenden Parabeln zu rekonstruieren.

## Vorgehensweise

1. Simulation von zwei Wurfparabeln  
2. Hinzufügen von Rauschen in x- und y-Richtung  
3. Vermischen der Messpunkte  
4. Erste Gruppierung der Punkte  
5. Quadratischer Fit für beide Gruppen  
6. Iterative Neuzuordnung der Punkte anhand ihres Abstands zu den gefitteten Parabeln  
7. Wiederholung des Verfahrens zur Verbesserung der Rekonstruktion  

## Beobachtungen

- Eine reine Trennung der Punkte in x-Richtung ist nicht ausreichend.
- Die iterative Neuzuordnung anhand des Abstands zur Parabel liefert deutlich bessere Ergebnisse.
- Zu starkes Rauschen verschlechtert die Rekonstruktion sichtbar.
- Zu viele Iterationen können kontraproduktiv sein.
- In den aktuellen Versuchen haben sich etwa 15 Durchläufe als sinnvoll erwiesen.

## Ziel des Projekts

Das Projekt dient als Einstieg in die Themen:
- Simulation von Trajektorien
- Clustering verrauschter Daten
- iterative Modellanpassung
- Rekonstruktion von Flugbahnen

## Ausblick

Als nächster Schritt soll das Verfahren auf weitere Bewegungsmodelle wie Vogel- oder Drohnenflug erweitert werden, um später auch eine Klassifikation verschiedener Flugobjekte zu ermöglichen.
