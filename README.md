# mindgraph-plugins

Offizieller Plugin-Katalog für [MindGraph Notes](https://mindgraph-notes.de).

`catalog.json` ist die **einzige** Quelle, die der In-App-Store liest (Discovery). Pro Eintrag:
`id`, `name`, `repo` (Pflicht) sowie optional `description`, `author`, `category`, `tag`.

Der Katalog ist **unsigniert** — er listet nur. Die Installation jedes Plugins prüft die **Ed25519-Signatur
gegen den in der App gepinnten Produktionsschlüssel**; nicht offiziell signierte Plugins werden abgelehnt.
Versions-/Update-Stand kommt live aus dem jeweiligen Plugin-Repo (GitHub-Releases).
