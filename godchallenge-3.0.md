# GodChallenge 3.0

GodChallenge 3.0 bündelt den geprüften Stand der Releases 2.1.123 bis 2.1.129 und räumt verbliebene Versions- und Menütexte auf. Spielstände, Welten, Konfigurationen und veröffentlichte Resourcepacks bleiben kompatibel.

## Spielerrelevante Inhalte

- MobArena: Runenkoloss, Glutmantis und Rissgeist besitzen eigene Java-Pack-Modelle, Texturen, Gelenkanimationen und angekündigte Spezialangriffe. Der Rissgeist rotiert zwischen Singularität, Schwerkraftumkehr und Rissnova.
- Die Träger-Trefferflächen folgen in 3.0 stärker der sichtbaren Größe: Koloss 1,35×, Mantis 1,18×, Rissgeist 1,20×. Modellteile wie einzelne Sicheln bleiben reine Dekoration. Ohne geladenes Pack und auf Bedrock bleibt der verlässliche Basismob sichtbar. In gemischten Runden kann er zusätzlich neben dem Modell sichtbar sein, damit kein Spieler einen unsichtbaren Gegner erhält.
- Dragon Run: zehn unterscheidbare Standardmodule mit eigenen Wegen, Höhenprofilen, Abzweigungen und Bauwerken; Wartungsmodus und Zuschauersystem sind angebunden.
- Menüs und Ergebnisse: gemeinsamer Einstieg über „Weiter spielen“, kürzere Texte, sichtbare Gratisstarts und Tokenkosten sowie einheitliche Ergebnisanzeigen.
- Fairplay: PvE erzeugt keine normalen KillAura-Snap-Wertungen; absichtliche Gravitationsimpulse werden ausschließlich für Bewegung kurz ausgenommen.

## Serverbasis

- Paper 26.2 Build 129 → 133. Offizieller SHA-256: `BF1DCF627364F8A631AB15250D240EB5A8E89FAAAC523B391E1C61367FCE9FF1`.
- ViaVersion 5.12.0 → 5.12.1. Offizieller SHA-256: `B8033807E7182C35003A45962352DD642C1E91880CA281DA3A43CB6F481A95A2`.
- ViaBackwards 5.12.0 → 5.12.1. Offizieller SHA-256: `29D94D3A26C85C8A327574B2322DB4078992AE457F0173325431A12AAC384911`.
- ViaRewind 4.2.0 ist bereits die aktuelle veröffentlichte Version. ProtocolLib meldet Unterstützung für Minecraft 26.2. Geyser unterstützt aktuell Java 26.2 und Bedrock bis 26.51.

Die JARs stammen von den offiziellen Paper- beziehungsweise ViaVersion-Projekten. Aktive Dateien werden erst nach lokalem Hashvergleich und FTP-Rückdownload ersetzt; die vorherigen Dateien bleiben als Rollback erhalten.

## Bekannte Grenze

Automatische Unit- und Paper-Integrationstests prüfen Logik, echte Entities, Packzustände, Animationstransformationen und Bereinigung. Sie ersetzen keinen Sicht- und Balance-Test mit verbundenen Java- und Bedrock-Clients. 3.0 behauptet deshalb keine vollständige Client-Abnahme.
