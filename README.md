# NamingConventions

| Oberbegriff                        | Begriff              | Übersetzung       | Erklärung                                                                                                                   | Beispiel                      | Zusatz                                                                                                            |
| ---------------------------------- | -------------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------------- | ----------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Daten erhalten/abfragen            |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | get                  | bekommen          | Liefert schnell einen Wert                                                                                                  | GetName()                     | Niemals asynchron                                                                                                 |
|                                    | compute              | berechnen         |                                                                                                                             |                               |                                                                                                                   |
|                                    | aquire               | erwerben          |                                                                                                                             |                               |                                                                                                                   |
|                                    | fetch                | abrufen           | Liefert Werte                                                                                                               |                               | Klingt nach mehr Aufwand als z.B.: get                                                                            |
|                                    | download             | herunterladen     |                                                                                                                             |                               |                                                                                                                   |
|                                    | retrieve             | abrufen           |                                                                                                                             |                               |                                                                                                                   |
|                                    | request              | anfordern         |                                                                                                                             |                               | Meistens asynchron                                                                                                |
|                                    | query                | Abfrage           |                                                                                                                             |                               | Synchron/Asynchron                                                                                                |
| Suchen/Beschaffen                  |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | find                 | finden            | Etwas gezielt suchen und zurückgeben.<br> Zum Beispiel einen Wert in Liste mit xyz                                          |                               |                                                                                                                   |
|                                    | search               | suche             | Etwas komplett durchsuchen

Zum Beispiel alle Werte in Liste mit xyz                                                        |                               | Search bedeutet nicht nach sonder in etwas suchen<br> searchFolder -> in Ordner suchen / nicht nach Ordner suchen |
|                                    | scan                 | durchsuchen       | Name deutet daraufhin, dass es länger dauert und alle Daten durchsucht (ähnlich wie search)                                 |                               |                                                                                                                   |
|                                    | seek                 | suchen            |                                                                                                                             |                               |                                                                                                                   |
| Beinhalte                          |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | include              | einschließen      |                                                                                                                             |                               |                                                                                                                   |
| Abgeben/Wiedergeben                |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | dump                 | abladen           |                                                                                                                             |                               |                                                                                                                   |
|                                    | render               | wiedergeben       |                                                                                                                             |                               |                                                                                                                   |
| Anzeigen/Ausblenden                |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | show                 | zeigen            | Etwas anzeigen                                                                                                              | ShowTooltip()                 | Nur verwenden wenn es auch eine hide-Funktion gibt                                                                |
|                                    | hide                 | ausblenden        | Etwas                                                                                                                       |                               | Nur verwenden wenn es auch eine show-Funktion gibt                                                                |
|                                    | display              | anzeigen          | Etwas darstellen                                                                                                            |                               | verwenden wenn es keine hide-Funktion gibt                                                                        |
| Verbindeb/Kombinieren/Verschmelzen |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | join                 | beitreten         | Kombiniert zwei Elemente miteinander ohne diese zu vermischen sondern zusammen zu fügen                                     | Path.Join()                   |                                                                                                                   |
|                                    | merge                | zusammenführen    | Erzeugt aus zwei Elementen ein Gesamtes<br> Zum Beispiel zwei Datenbanktabellen kombinieren / Git merge                     |                               |                                                                                                                   |
|                                    | combine              | mischen           | Erzeugt aus zwei Elementen ein Gesamtes (wie merge aber mit Unschärfe. Merge beinhaltet mehr Logik)                         |                               |                                                                                                                   |
| Anfügen                            |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | prepend              | vorangestellt     | Etwas vor ein Element anfügen (z.B.: Präfix)                                                                                |                               |                                                                                                                   |
|                                    | append               | anhängen          | Etwas hinter ein Element anfügen (z.B.: Suffix)                                                                             |                               |                                                                                                                   |
|                                    | concat (concatenate) | verketten         |                                                                                                                             |                               |                                                                                                                   |
|                                    | expand               | erweitern         |                                                                                                                             |                               | Gegenteil: collapse                                                                                               |
| Zerlegen                           |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | split                | geteilt           | Teilt etwas in mehrere Teile                                                                                                |                               | Gegenteil: Join                                                                                                   |
|                                    | slice                | schneiden         | Etwas herausschneiden                                                                                                       |                               |                                                                                                                   |
|                                    | splice               | verbinden         | Etwas herausschneiden und ein neues Element in die Lücke einfügen                                                           |                               |                                                                                                                   |
| Umwandeln                          |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | parse                | zerlegen          | Zerteilt etwas in sinnvolle Elemente (z.B.: JSON-Object)                                                                    | JSON.Parse()                  |                                                                                                                   |
|                                    | serialize            | anordnen          | Wandelt Objektdaten in eine andere Struktur (z.B.: Objekt in JSON umwandeln)                                                |                               | Alternative: stringify<br> Gegenteil: deserialize/unserialize                                                     |
|                                    | stringify            | \-                | Wandelt Objektdaten in eine andere Struktur (z.B.: Objekt in JSON umwandeln)                                                |                               | Alternative: serialize

Gegenteil: deserialize/unserialize                                                        |
|                                    | deserialize          | auftrennen        | Wandelt Daten in Objekte um (z.B.: JSON-String in Objekt)                                                                   |                               | Alternative: unserialize<br> Gegenteil: serialize/stringify                                                       |
|                                    | unserialize          | \-                | Wandelt Daten in Objekte um (z.B.: JSON-String in Objekt)                                                                   |                               | Alternative: deserialize<br> Gegenteil: serialize/stringify                                                       |
|                                    | to                   | zu                | Kurzform für eine Konvertierung (Umwandlung in anderes Objekt)                                                              | toHTML(), toJPG(), toString() |                                                                                                                   |
|                                    | convert              | umwandeln         | Konvertierung (Umwandlung in anderes Objekt)                                                                                | ConvertToBase64String()       |                                                                                                                   |
|                                    | invert               | umkehren          | Kehrt die Reihenfolge oder Richtung um                                                                                      |                               |                                                                                                                   |
|                                    | reverse              | umkehren          | Wandelt in das Gegenteil um

(positiv <-> negativ, Hell <-> Dunkel)                                                         |                               |                                                                                                                   |
| Anfangen/Beenden                   |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | start                | starten           |                                                                                                                             | Process.Start()               | Nicht vermischen<br>Richtig: start -> stop<br> Falsch: start -> end                                               |
|                                    | stop                 | aufhören          |                                                                                                                             | Process.Stop()                | Nicht vermischen<br>Richtig: start -> stop<br> Falsch: begin -> stop                                              |
|                                    | begin                | anfangen          |                                                                                                                             |                               | Nicht vermischen<br>Richtig: begin -> end<br> Falsch: begin -> stop                                               |
|                                    | end                  | beenden           |                                                                                                                             |                               | Nicht vermischen<br>Richtig: begin -> end<br> Falsch: start -> end                                                |
|                                    | open                 | öffnen            |                                                                                                                             | OpenWindow()                  | Gegenteil: close                                                                                                  |
|                                    | close                | schließen         |                                                                                                                             | CloseWindow()                 | Gegenteil: open                                                                                                   |
|                                    | pause                | unterbrechen      |                                                                                                                             | PauseMusic()                  | Gegenteil: resume                                                                                                 |
|                                    | resume               | fortsetzen        |                                                                                                                             | ResumeMusic()                 | Alternative: play

Gegenteil: pause                                                                               |
|                                    | play                 | fortsetzen        |                                                                                                                             |                               | Alternative: resume

Gegenteil: pause                                                                             |
|                                    | exit                 | verlassen         |                                                                                                                             | Application.Exit()            |                                                                                                                   |
|                                    | construct            | bauen             |                                                                                                                             |                               | Gegenteil: desctruct                                                                                              |
|                                    | descruct             | abbauen           | Geregelter/sanfter Abbau von etwas                                                                                          |                               | Alternative: destroy & kill

Gegenteil: construct                                                                 |
|                                    | destroy              | zerstören         | Härterer Abbau als destruct                                                                                                 |                               | Alternative: destruct & kill                                                                                      |
|                                    | kill                 | töten             | Härteste Variante für den Abbau                                                                                             | Task.Kill()                   | Alternative: destruct & destroy                                                                                   |
| Aufräumen/Umräumen                 |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | buffer               | puffern           | Zwischenspeichern von Daten (z.B.: im Cache)                                                                                |                               |                                                                                                                   |
|                                    | flush                | spülen            | Leert etwas aber so, dass es weiterverwendet werden kann<br> (z.B.: Cache Daten in festen Speicher übermitteln)             | FlushCache()                  | Alternative: clear & purge                                                                                        |
|                                    | clear                | leeren            | Leert etwas ohne Rücksicht auf Verluste (Hauptsache Weg)                                                                    | ClearFilters()                | Alternative: flush & purge                                                                                        |
|                                    | purge                | bereinigen        | Gleich wie clear aber härtere Formulierung                                                                                  | PurgeTempTables()             | Alternative: flush & clear                                                                                        |
|                                    | cleanup              | Aufräumen         | Unvollendete Vorgänge werden beendet                                                                                        | CleanTempFiles()              |                                                                                                                   |
|                                    | collapse             | zusammenfalten    | Etwas Platzraubendes zusammenfalten                                                                                         | CollapseNavigation()          | Gegenteil: expand                                                                                                 |
|                                    | compact              | verdichten        | Etwas zusammenfalten aber so, dass es unumkehrbar ist                                                                       | CompactDatabase()             |                                                                                                                   |
|                                    | move                 | bewegen           | z.B.: Umzug von Datei von Verzeichnis A nach B                                                                              | MoveFile()                    |                                                                                                                   |
|                                    | tidy                 | säubern           |                                                                                                                             | TidyHTML()                    | Gegenteil: minify & uglify                                                                                        |
|                                    | pretty               | aufhübschen       |                                                                                                                             | PrettyPrint()                 | Gegenteil: minify & uglify                                                                                        |
|                                    | beautify             | verschönern       |                                                                                                                             | BeautifyJSON()                | Gegenteil: minify & uglify                                                                                        |
|                                    | minify               | verkleinern       |                                                                                                                             |                               | Gegenteil: tidy & pretty & beautify                                                                               |
|                                    | uglify               | hässlich machen   |                                                                                                                             |                               | Gegenteil: tidy & pretty & beautify                                                                               |
| Speichern/Festlegen                |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | save                 | speichern         | Gibt Daten in dauerhaften Speicher ab                                                                                       | SaveToFile()                  | Alternative: Store                                                                                                |
|                                    | store                | speichern         | Gibt Daten in dauerhaften Speicher ab                                                                                       | StoreResult()                 | Alternative: Save                                                                                                 |
|                                    | write                | schreiben         | Kann auch etwas ausgeben ohne die Absicht diese dauerhaft zu erhalten                                                       | Console.Write()               |                                                                                                                   |
|                                    | commit               | übergeben         | Verwendung bei Transaktionen                                                                                                | CommitNewItems()              |                                                                                                                   |
|                                    | bake                 | \-                | Vorgang der länger dauert. Brennt etwas dauerhaft ein                                                                       |                               |                                                                                                                   |
| Rückgängig machen                  |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | redo                 | wiederherstellen  |                                                                                                                             |                               | Gegenteil: undo                                                                                                   |
|                                    | undo                 | rückgängig machen |                                                                                                                             | UndoMove()                    | Nach undo sollte ein Verb folgen<br> Gegenteil: redo                                                              |
|                                    | rollback             | zurücksetzen      | Umfangreichere Operation. Es werden bisherige Arbeitsschritte rückgängig gemacht                                            | RollbackPatch()               |                                                                                                                   |
|                                    | restore              | wiederherstellen  | Früheren Stand oder Default-Stand herstellen (Gespeicherter Zustand)                                                        | RestoreSettings()             |                                                                                                                   |
|                                    | revert               | zurückgehen       | Vorgenommene Änderung zurücksetzen (Nicht gespeicherter Zustand)                                                            | RevertAllChanges()            |                                                                                                                   |
|                                    | recover              | zurückgewinnen    | Kommt in Ausnahmesituationen zum Einsatz wenn man **versucht** etwas wiederherzustellen                                     | RecoverSession()              |                                                                                                                   |
| Nicht verwenden (Vorsicht)         |                      |                   |                                                                                                                             |                               |                                                                                                                   |
|                                    | process              | Vorgang           |                                                                                                                             |                               |                                                                                                                   |
|                                    | do                   | tun               |                                                                                                                             |                               |                                                                                                                   |
|                                    | perform              | durchführen       |                                                                                                                             |                               |                                                                                                                   |
|                                    | dealWith             | behandeln         |                                                                                                                             |                               |                                                                                                                   |
|                                    | manage               | verwalten         |                                                                                                                             |                               |                                                                                                                   |
|                                    | change               | ändern            |                                                                                                                             |                               |                                                                                                                   |
|                                    | handle               | behandeln         |                                                                                                                             |                               |                                                                                                                   |
|                                    | resolve              | beheben           |                                                                                                                             |                               |                                                                                                                   |
|                                    | filter               | filtern           |                                                                                                                             |                               | Alternativen: select & find & extract & reject & exclude & strip                                                  |
|                                    | check                | überprüfen        | Anweisung: Pass auf ob die Milch überkocht!<br> Check: Ich habe genau aufgepasst. Es war halb zwölf als es übergekocht ist. |                               | Besser z.B.: IsValid() verwenden                                                                                  |
|                                    | validate             | bestätigen        |                                                                                                                             |                               |                                                                                                                   |
|                                    | verify               | überprüfen        |                                                                                                                             |                               |                                                                                                                   |
|                                    | test                 | testen            |                                                                                                                             |                               |                                                                                                                   |
