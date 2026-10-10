# Rissgeist: Gravitationsangriffe – 2.1.129

Der Rissgeist rotiert durch drei Angriffe. Jeder markiert die zum Start festgehaltene Spielerposition zwei Sekunden vorher. Während dieses Aufladens unterbrechen zusammen 8 % seiner maximalen Lebenspunkte den Angriff. Nach einer beendeten Fähigkeit folgen 8,5 Sekunden Pause bis zur nächsten Warnung.

| Angriff | Verhalten |
|---|---|
| Singularität | Radius 4,5 Blöcke. Drei Sekunden leichter Sog, danach eine Druckwelle. Der Impuls erfolgt alle sechs Ticks; Springen und Gegensteuern bleiben möglich. |
| Schwerkraftumkehr | Radius 3 Blöcke. Ein leichter Hub pro getroffenem Spieler, danach kurze gedämpfte Vertikalbewegung für insgesamt 1,2 Sekunden. Drei Sekunden langsames Fallen ab dem letzten Impuls schützen die Landung. Danach eine Druckwelle. |
| Rissnova | Radius 3 Blöcke. Nach der Warnung sofortiger Flächentreffer; der Geist führt seinen seitlichen Ausweichimpuls aus. |

Nur der Abschluss verursacht Schaden: `min(8, 3 + Welle × 0,15)` Schadenspunkte vor Schadensreduktion. Wer das Feld rechtzeitig verlässt, entgeht diesem Schaden. Die vertikale Reichweite beträgt ±3 Blöcke. Spieler hinter einer Sichtblockade zum Geist werden weder bewegt noch vom Abschluss getroffen. Zuschauer, Spieler in anderen Welten und niedergeschlagene Teilnehmer sind ausgenommen.

Jeder Gravitationsimpuls gewährt zwei Sekunden Fairplay-Ausnahme ausschließlich für Bewegung. Es gibt keine Teleports und keine globale Abschaltung der Prüfungen. Der horizontale Sog ist auf 0,38 begrenzt; der erste Hub auf 0,32, weitere Vertikalimpulse auf ±0,08. Slow Falling läuft regulär aus, damit beim Abbruch keine ungeschützte Landung entsteht. Bestehende längere oder stärkere Effekte werden über Bukkits reguläre Effektpriorität erhalten.

Die Felder gehören ihrem erzeugenden Mob und ihrer Welle. Entfernte/tote Erzeuger, Wellenwechsel, abgebrochene Fähigkeiten und Rundenbereinigung beseitigen sie. Es werden keine zusätzlichen wiederkehrenden Tasks erstellt; die bestehende Zwei-Tick-Aufgabe aktualisiert die Felder.

Das Resourcepack 2.1.128 bleibt unverändert gültig: Die vorhandenen animierten Schwingen und schwebenden Modellteile werden weiterverwendet. Ein erneuter Pack-Upload ist für diese Angriffe nicht erforderlich.
