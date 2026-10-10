# Eigene Mob-Modelle und Texturen – 2.1.128

2.1.128 ersetzt die Vanilla-Blockdarstellung aus dem nur lokal gebauten Stand 2.1.127. Runenkoloss, Glutmantis und Rissgeist besitzen jetzt 46 eigene Modellteile mit skulptierten Panzerplatten, Kristallspitzen, Sicheln und zerrissenen Mantelteilen. Sämtliche neuen Flächen verwenden einen eigenen Texturatlas, keine Minecraft-Blocktexturen. Der alte Runenwächter-Kopf bleibt für ältere Plugin-Versionen im Pack enthalten.

Die vorhandenen Lauf-, Schwebe-, Schwingen- und Angriffsanimationen steuern Item-Display-Gelenke. Modellteile haben keine zusätzliche Trefferfläche. Minecraft-Blocktexturen werden auch dann nicht als Ersatzmodell angezeigt, wenn ein Pack fehlt.

Das optionale Pack wird beim Betreten der MobArena angeboten. Erst SUCCESSFULLY_LOADED schaltet die Modellteile für den jeweiligen Spieler frei. Laden, Ablehnen, Entfernen oder fehlende Unterstützung führen zu einem sichtbaren Basismob. In gemischten Runden bleibt dieser gemeinsame Basismob zusätzlich für Pack-Nutzer sichtbar; die eigenen Modellteile sehen nur Spieler mit geladenem Pack. Bedrock und ältere Java-Versionen erhalten weiterhin den Basismob. Das ist kein Bedrock-Custom-Entity-Pack.

Der sichtbare Gegner besitzt weiterhin die Zombie-Trefferfläche. Breite Schultern und Sicheln sind Dekoration. Die zehn überarbeiteten Dragon-Run-Strecken aus 2.1.127 sind enthalten.

## Pack und Veröffentlichung

- Versionierter Download: `godchallenge-custom-mobs-2.1.128.zip` im Repository `bengessert-ui/godchallengePUPLIC`.
- Manifest: `custom-mobs-2.1.128.json` enthält URL, SHA-1, Größe und Zielversion.
- Bestehende Pack-URLs werden nicht überschrieben.
- `creaturePackAssets` erzeugt Modell- und Item-JSONs aus dem gemeinsamen Skelett; `resourcepack/release-creatures.ps1` baut das ZIP und aktualisiert ausschließlich den Custom-Mob-Abschnitt der Plugin-Packkonfiguration.
- `creaturePreview` rendert die exportierte Geometrie mit dem Texturatlas als neutrale Vorschau. Dies ist kein Screenshot aus Minecraft und keine visuelle Client-Abnahme.

## Texturherkunft

Der Atlas `resourcepack/custom-mobs/assets/godchallenge/textures/entity/arena_creatures.png` wurde mit dem eingebauten Imagegen-Werkzeug erstellt. Prompt: ein flacher 3×3-Atlas eigener Dark-Fantasy-Materialien; Spalten Runenrüstung/türkiser Kristall/dunkle Gelenke, glühender Insektenpanzer/bernsteinfarbene Sichel/rote Chitinsegmente und violetter Geisterstoff/lila Kristall/sternbestickter Mantel; keine Vanilla-Texturen, Beschriftungen oder Perspektive. Die Originaldatei bleibt im Imagegen-Ausgabeordner erhalten.

Technische Grundlage: [Minecraft Item-Modelle](https://www.minecraft.net/fr-fr/article/minecraft-java-edition-1-21-4), [Paper Display-Entities und Sichtbarkeit](https://docs.papermc.io/paper/dev/display-entities/).
