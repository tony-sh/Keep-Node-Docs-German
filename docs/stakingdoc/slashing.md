# Reduzierung und Beseitigung
Die Abkürzung in Keep- und tBTC-Systemen soll nicht bestrafen, sondern die Netzwerksicherheit vor böswilligem Verhalten schützen.
## Was ist Abkürzung?
Downsizing ist eine Strafe für Fehlverhalten von Gruppen. Dadurch wird ein Teil Ihrer delegierten KEEP-Token entfernt (normalerweise ein Mindestgebot). Wenn Sie einen Absteckanbieter verwenden, müssen Sie sich keine Gedanken über Kürzungen machen.
Kontraktionsvektoren sind minimal und nur dann strafbar, wenn der Verdacht auf böswilliges Verhalten besteht. Solange die Random Beacon-Gruppe (64 Unterzeichner) die Aufzeichnung erstellt, werden Sie nicht beschnitten, wenn Sie Ausfallzeiten hatten und Teil der Gruppe waren, die für die Erstellung der Aufzeichnung ausgewählt wurde.

Das verringerte Verfügbarkeitsrisiko korreliert mit der Anzahl der gespeicherten Gruppen oder Unterzeichnergruppen, zu denen jeder Betreiber (Kunde) gehört.

## Abkürzungsvektoren in Keep
Angenommen, Sie haben 500.000 KEEP.

Sie können alle Ihre Eier (Delegierter) in einen Korb legen (Betreiber / Kunde). Dies bedeutet, dass jede von Ihnen ausgewählte Unterzeichnergruppe verfügbar ist. In diesem Szenario berechnen Sie alle Ihre 500.000 KEEPs pro Kunde.

Angenommen, Ihr Kunde gehört 10 Unterzeichnergruppen an, und 3 dieser Gruppen erhalten einen Anruf, während Sie nicht arbeiten. In diesen Fällen erfolgt keine Eingabe und der Mindesteinsatz wird um das Dreifache reduziert.

Nun, wie Matt gerne betont ... Nehmen wir an, Sie haben Ihre Eier (KEEP) auf mehrere Körbe (Betreiber / arbeitende Kunden) verteilt, mit einem Mindestgebot (100.000) pro Kunde. Sie befinden sich jetzt in einer Situation, in der die gespeicherten Gruppen oder Unterzeichnergruppen, an denen Sie teilnehmen, auf 5 eindeutige Clients im Netzwerk verteilt sind. Dies sollte die Wahrscheinlichkeit verringern, dass Sie abgelehnt werden, indem Sie eine Sicherungsgruppe oder Signatur auf mehrere Clients verteilen.

Wenn ein Rechenzentrumsfehler auftritt, werden alle Ihre Clients offline geschaltet, und Sie müssen immer noch im Geiste des ersten Szenarios in diesem Beitrag leiden.


## Vektoren von tBTC-Abkürzungen
In tBTC tritt die Kürzung nur im Fall von böswilligem Verhalten auf, d.h. wenn Unterzeichner mit Bitcoins abreisen. Es gibt jedoch Strafen für Nichtverfügbarkeit.

Es gibt Zeitüberschreitungen für angeforderte Transaktionen, wie z. B. Rücknahmen, die dazu führen können, dass Anleihen beschlagnahmt und liquidiert werden. Im Keep-System verlieren Sie mindestens 1 KEEP, wenn nicht genügend Unterzeichnergruppen verfügbar sind, um bei Auswahl einen Datensatz zu erstellen. In tBTC verlieren Sie alle Ihre ETH-Sicherheiten, wenn Sie bei Bedarf nicht verfügbar sind.

Die Risiken einer Platzierung der ETH auf tBTC hängen hauptsächlich mit Währungsrisiken zusammen. Im Vergleich zum Einsatz mit einem zufälligen Random Beacon verfügt t-ECDSA tBTC über einige zusätzliche Funktionen außerhalb der Kette, die gesteuert werden müssen. Das Hauptszenario besteht darin, eine Liquidation zu verhindern. Wenn der Preis der ETH stark sinkt, vergleichbar mit BTC, müssen Sie bereit sein, Ihre Einzahlung einzulösen und an Auktionen teilzunehmen, um einen "Flop" zu vermeiden. Wir haben einige interne Skripte dafür. Dieses Problem wird bis zum 8. Juni behoben sein, aber einige der größeren ETH-Unterzeichner arbeiten mit uns zusammen, um sicherzustellen, dass die Skripte hier hervorragend funktionieren.

Die „Reduzierung“ der ETH-Sicherheiten wird im tBTC-System als Liquidation bezeichnet, und es gibt viele Warnungen und Möglichkeiten, die Liquidation rechtzeitig vor der Auktion zu verhindern.

## tBTC - Liquidation der BTC / ETH
In diesem Fall erfolgt die Liquidation von tBTC in Form einer langsamen langfristigen Auktion mit fallendem Preis. Die Liquidation wird frühzeitig und absichtlich gestartet, damit Sie die Auktion ohne wesentlichen "Fehler" beenden können. Das größte Risiko bei einer tBTC-Liquidation wäre daher der Verlust einiger Basispunkte aufgrund eines "Einbruchs".

Wenn Ihre Sicherheiten in Liquidation mit 125% unterbesichert sind, werden Sie vom System von Teilnehmern abgeschnitten, die kommen und ihre Sicherheiten mit zusätzlicher ETH auffüllen. Jeder der Unterzeichner hat die Möglichkeit, die Anzahlung abzuheben und zu schließen.

Die Reduzierung der Ausfallzeiten im tBTC-System ist recht gering und für einen fortgeschrittenen Staker nahezu vernachlässigbar. Wenn Sie bei Erhalt Ihrer Signaturanfrage nicht verfügbar sind, haben Sie 6 bis 24 Stunden Zeit, um die Anfrage zu bearbeiten, bevor Sie verkleinert werden.

Der Schutz von Bitcoin vor böswilligem Verhalten ist eine Funktion des Systems. Daher ist die Kontraktion der einzig wirklich wirksame Parameter.

## Wie die Schließung von tBTC-Einzahlungen funktioniert

Alle Optionen zum Schließen von Einzahlungen führen dazu, dass 1 TBTC an den TDT-Inhaber übertragen wird. Alle abgebauten TBTCs stammen von TDT. Die Kosten betragen 1 TBTC + Signiergebühr (schwierig, aber vereinfacht). Dieser 1 TBTC geht an den TDT-Halter (es sei denn, der TDT-Halter kauft ihn zurück).


`Entnommen aus der offiziellen Dokumentation von Keep Team.` [Quelle] (https://keep-network.gitbook.io/staking-documentation/)

## Mehr Informationen :
- State Layer [Dokument über Stakedrop-Risiken aufbewahren] (https://hackmd.io/@LayerState/KeepStakedropRisks)
- Risikominderung auf dieser Website [hier (Englisch)] (Node-Operation / risks.md)

"Autoren: Ramaruro, EstebanK"
`Übersetzung: nadyakriy`
