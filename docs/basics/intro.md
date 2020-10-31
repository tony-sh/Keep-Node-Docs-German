# Einführung in tBTC & Keep Network


## DeFi
Decentralized Finance (DeFi) ist ein System offener und miteinander verbundener Finanzdienstleistungen und -produkte, die im Ethereum-Netzwerk aufgebaut und betrieben werden. Bis Juli 2020 sind fast 4 Milliarden US-Dollar an allen DeFi-Anträgen beteiligt, die Kredite, Token, Derivate und Börsen über dezentrale Smart-Verträge anbieten. Dieses Volumen wächst weiter.

DeFi-Protokolle sind modular aufgebaut, sodass sie miteinander interagieren können, wodurch ein zunehmend komplexeres System entsteht. Da es sich bei DeFi-Produkten um Code handelt, der sich in einem Blockchain-Netzwerk wie Ethereum befindet, können sie niemals deaktiviert oder vor Personen verborgen werden, die sie verwenden möchten. Somit kann jeder mit Internetzugang von Krediten, umfassenden Finanzprodukten, Spar-, Investitions- und Handelsmöglichkeiten auf DeFi profitieren.

## Absichten tBTC
Trotz des exponentiellen Wachstums der Projekte in DeFi und Ethereum macht Bitcoin immer noch zwei Drittel der gesamten Kryptowährung der Welt aus.

Wie Ilyas Khatsis tBTC in seinem [Blog] vorstellt (https://medium.com/@iliashatzis/could-bitcoin-on-defi-displace-banks-yes-4c0ad99f0da4):
> „Bitcoin DeFi ist der Traum von Bitcoinern. Wir können davon träumen, dass das neue tBTC-Projekt Bitcoin in die DeFi-Welt bringt.
> Bitcoin hat das Potenzial, DeFi dramatisch zu verändern, und das Keep-Team versteht das. “

Das Keep-Team hat tBTC eingeführt, ein dezentrales, sicheres und versichertes Speichersystem für Bitcoins in TBTC Ethereum ERC-20-Token mit einer 1: 1-Rate für BTC. Bitcoin-Inhaber, die ihre BTC für Ethereum und DeFi ausgeben möchten, sollten den Depotbanken (Unterzeichnern) nicht vertrauen, da die Unterzeichner Sicherheiten hinterlegen müssen, die über den Wert der von ihnen verwahrten BTC hinausgehen.

?> Ausgezeichnetes [Video] (https://www.youtube.com/watch?v=cfmQiArg3B8) dazu von Artem # 4718 auf Discord.

Die Unterzeichner werden zufällig aus dem größeren Netzwerk der Unterzeichner ausgewählt und arbeiten in Dreiergruppen. Sicherheiten stellen sicher, dass das Verhalten der Unterzeichner im System fair bleibt und das Risiko besteht, dass ihre Sicherheiten bei Betrug oder unzureichenden Sicherheiten verloren gehen. Wenn die Unterzeichner Gelder ohne Genehmigung bewegen und mehr TBTC in Verwahrung lassen als BTC, beschlagnahmt das System ihre Sicherheiten, um das TBTC-Äquivalent vom Markt zu kaufen und zu zerstören, wodurch die TBTC- und BTC-Bestände ins Gleichgewicht gebracht werden.

<p align = "center">
  <img width = "619" alt = "Beacon" src = "https://user-images.githubusercontent.com/68087535/88100735-57075f80-cb73-11ea-996f-ec2d9590b073.png">
</ p>


## Netzwerk behalten

tBTC ist eine Anwendung bei [Keep Network] (https://keep.network), die Ben Longstaff mit einer ausgezeichneten [Beschreibung] (https://medium.com/@ben_longstaff/secure-multi-party-computation) versehen hat -smpc-erklärt-visuell-ecde155fc7c0):

> „Keep Network soll eine Datenschutzlösung für die sichere Speicherung von Daten außerhalb des Netzwerks werden und gleichzeitig die Funktionalität intelligenter Verträge und die Masseneinführung der Blockchain-Technologie erheblich erweitern.“

Keep Network ist eine Datenschutzlösung, die verteilte kleine Datenmengen wie einen privaten Schlüssel speichert und die Kommunikation zwischen den Ketten aufrechterhält. Keeps sind intelligente Verträge, mit denen andere intelligente Verträge sicher mit personenbezogenen Daten interagieren können. Sie basieren auf dem ECDSA-Algorithmus, der von vielen führenden Blockchains unterstützt wird, und erleichtern das Signieren dezentraler Gruppen mithilfe von Mehrparteien-Schwellenwertsignaturen.

Keep Network at [Messari] (https://messari.io/article/announcement-messari-adds-11-new-disclosures-registry-participants-surpassing-50-members) ist ein offenes registriertes Mitglied. Durch den Beitritt zu diesem Hauptbuch haben sich diese Projekte dazu verpflichtet, die Transparenz von Kryptoassets durch kontinuierliche Offenlegung zu erhöhen.

[Keeps Grants Explorer] (https://explorer.keep-grants.info/) von MutedTommy # 3155 (in Discord) verfolgt die von KEEP zugewiesenen Zuschüsse in Token.

### t-ECDSA-Knoten

T-ECDSA keep bietet Transaktionssicherheit mit mehreren privaten Schlüsseln, die von mehreren Unterzeichnern gehalten werden. Die dezentrale Signatur wird mit sMPC (Secure Multiparty Computing) ausgeführt, um gemeinsam genutzte Schlüssel zu berechnen, ohne sie verfügbar zu machen. Die Verantwortung für Signaturen ist aufgeteilt und erfordert eine bestimmte Anzahl von Teilnehmern, um eine Signatur zu erstellen.

Im Allgemeinen funktioniert es so: Der Ethereum-Smart-Vertrag fordert das Keep-Netzwerk auf, eine neue t-ECDSA-Festung zu eröffnen. Dieser Speicher wird von einer Gruppe zufällig ausgewählter Unterzeichner aus dem sMPC-Cluster, einem größeren Netzwerk von Unterzeichnern, verwaltet. Diese Unterzeichner verwenden t-ECDSA, um einen Schlüssel zu generieren und eine Signatur bereitzustellen. Unterzeichner können alles signieren, einschließlich Blockchain-Transaktionen. Ein Ethereum-Smart-Vertrag kann Keep auffordern, eine Transaktion für eine ECDSA-basierte Blockchain zu unterzeichnen. Bitcoin ist nur eine davon.

Dieser Mechanismus ist zuverlässig, da die Unterzeichner unabhängig sind. Dies sind Personen und Organisationen, die einen Knoten mit einem sMPC-Cluster gestartet haben.

<p align = "center">
  <img width = "319" alt = "Beacon" src = "https://user-images.githubusercontent.com/68167410/88845610-05ca2200-d1aa-11ea-9d8b-400516fed25c.png">
</ p>

### Random Beacon-Knoten

Random Beacon ist ein weiterer Teil des Netzwerks: ein dezentrales Tool zur zufälligen Auswahl von Unterzeichnern. Dieses Leuchtfeuer ist BLSThreshold Relay und kann nicht gesteuert oder manipuliert werden. Es ist eine zuverlässige Zufallsquelle für die Gruppenauswahl. Niemand weiß, wer die Unterzeichner sein werden, einschließlich der Unterzeichner selbst, bis sie von einem zufälligen Leuchtfeuer ausgewählt werden. Dies stellt sicher, dass Unterzeichner nicht zusammenarbeiten können, um Geld zu stehlen oder das Netzwerk anzugreifen, weshalb die wahre Zufälligkeit des Beacons so wichtig ist.

** Random Beacon und t-ECDSA Hält den Kern im Keep-Netzwerk. **



***.

** Quellen und nützliche Informationen: **
- [Könnte Bitcoin auf DeFi Banken verdrängen? Ja] (https://medium.com/@iliashatzis/could-bitcoin-on-defi-displace-banks-yes-4c0ad99f0da4) von Ilias Hatzis
- [Bridging Bitcoin and Ethereum] (https://blog.keep.network/bridging-bitcoin-and-ethereum-b2f9923630a7) aus dem Keep Network Blog
- [Secure Multiparty Computation] (https://medium.com/@ben_longstaff/secure-multi-party-computation-smpc-explained-visually-ecde155fc7c0) von Ben Longstaff
- [Brücken bauen zwischen Blockchains mit tECDSA-Keeps] (https://blog.keep.network/building-bridges-between-blockchains-with-t-ecdsa-keeps-e58d6debb8fd) von Piotr Dyraga aus dem Keep Network Blog
- [Staking Documentation] (https://keep-network.gitbook.io/staking-documentation/) aus der Keep Network Documentation
- [tBTC Technical Overview] (https://tbtc.network/developers/tbtc-technical-system-overview/) von der tBTC-Website
- [Was ist in einem Leuchtfeuer?] (Https://blog.keep.network/whats-in-a-beacon-12c34b0bc078) von Antonio Salazar Cardozo aus dem Keep Network Blog
- [Warum ist vertrauenswürdige Zufälligkeit so wichtig?] (Https://blog.keep.network/why-is-trusted-randomness-so-important-c22de1c1c5ee) von Antonio Salazar Cardozo aus dem Keep Network Blog
- [Threshold ECDSA - Sicherere, privatere Mehrfachsignaturen] (https://blog.keep.network/threshold-ecdsa-safer-more-private-multi-signatures-51153f3e9ed2) von Antonio Salazar Cardozo aus dem Keep Network Blog on Halten Sie die Präsentation von Entwickler Piotr Dyraga zu Schwellen-ECDSA aus der San Francisco Blockchain Week 2018 aufrecht.
- [Defi erklärt] (https://decrypt.co/resources/defi-decentralized-finance-explained-guide-learn) von Decrypt.co
- [Was ist Defi] (https://defipulse.com/blog/what-is-defi/) von Defipulse
- [Promo-Video behalten] (https://www.youtube.com/watch?v=h2IErqf-VrQ) von Lelka Bo im Discord Design Channel
- [TBTC: Ein neues Sidechain-Design für Bitcoin] (https://insights.deribit.com/market-research/a-new-sidechain-design-for-bitcoin/) von Su Zhu in Deribit Insights
- Die Bilder stammen von SpaceWalker (Discord Design Channel), [Ilias Hatzis] (https://medium.com/@iliashatzis) (aus seiner Geschichte), Keep Team (Discord Design Channel).

--- ---.
`Quelle aus der offiziellen Keep Team-Dokumentation, die von der Community bearbeitet und hinzugefügt wurde. '[Quelle] (https://keep-network.gitbook.io/staking-documentation/) `

"Autoren: Ramaruro, EstebanK"
`Übersetzung: nadyakriy`
