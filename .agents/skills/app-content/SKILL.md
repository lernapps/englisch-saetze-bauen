---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

„Sätze bauen: Aussage, Frage und Verneinung mit do“: Explainer (Strang-App `englisch/grammatik`, Format 2, Sprache Deutsch, englische Beispiele) über Wortstellung, Imperativ, Fragen, Verneinung mit dem Helfer do, Kurzantworten und question tags. Auftrag: Issue lernapps/apps#473 (Epic lernapps/apps#489, Konventionen dort). Die erste Version baut nur Stufe 5-6 (Kapitel 1 bis 3); Kapitel 4 „Betonen und umstellen“ (Stufe 9-10: `emphase-do`, `inversion`) ist das Inkrement `increment/04-stufe-9-10`.

## Curriculum

Englisch als erste Fremdsprache, Klasse 5-6 (erstes und zweites Lernjahr, Stufe 5-6 der Karte). Kein Lehrplan: Reihenfolge und Bausteine kommen aus der Lernlandkarte `https://lernapps.net/apps/map/englisch.json` (Fokus `competency`; Strang-App des Strangs `grammatik`). Vorwissen: Hello, Millbrook! (#470, `classroom-phrases`) und Zeiten auf dem Zeitstrahl (#472: `to-be`, `simple-present`, `simple-past`). Nicht hier: die Zeitformen selbst (#472), Nebensätze, indirekte Rede und indirekte Fragen (#481), Satzmelodie der Frage (#482), Stellung der Adverbien (#476), Modalverben in Fragen und question tags, Kapitel 4 (Inkrement).

## Competencies

Alle neun sind Lücken der Karte, Band 5-6. Eine Seite je Baustein, Ordnung nach `requires`. Von außen braucht die Karte `classroom-phrases`, `simple-present`, `to-be` und `simple-past`: sie stehen als Sammel-Wiederholung (`recap`) am Kapitelanfang.

1. Kapitel `aussage-und-aufforderung` („Aussage und Aufforderung“)
   - Wiederholung `recap: englisch/classroom-phrases` → `aussage-und-aufforderung/das-brauchst-du` (ohne Übung)
   - `wortstellung` → `aussage-und-aufforderung/wortstellung`
   - `imperativ` → `aussage-und-aufforderung/imperativ` (don't als erster Helfer)
2. Kapitel `fragen-mit-do` („Fragen und verneinen mit do“)
   - Wiederholung `recap: [englisch/simple-present, englisch/to-be]` → `fragen-mit-do/das-brauchst-du`
   - `simple-present-fragen` → `fragen-mit-do/do-und-does` (Musterseite)
   - `kurzantworten` → `fragen-mit-do/kurzantworten`
   - `fragewoerter` → `fragen-mit-do/fragewoerter`
   - `subjektfragen` → `fragen-mit-do/subjektfragen`
   - `fragen-praeposition-ende` → `fragen-mit-do/praeposition-am-ende`
3. Kapitel `did-und-tags` („did und question tags“)
   - Wiederholung `recap: englisch/simple-past` → `did-und-tags/das-brauchst-du`
   - `simple-past-fragen` → `did-und-tags/did`
   - `question-tags` → `did-und-tags/question-tags`

4. Kapitel `betonen-und-umstellen` („Betonen und umstellen“, Stufe 9-10; keine Wiederholungsseite, alle `requires` übt die App schon)
   - `emphase-do` → `betonen-und-umstellen/emphase-do` (Musterseite der Stufe 9-10, Lesestück Marie Curie)
   - `inversion` → `betonen-und-umstellen/inversion` (Lesestück Mondlandung Apollo 11)

Die „Ich kann“-Sätze stehen in `src/<kapitel>/<seite>.yaml` wie in der Karte (nicht umformulieren). Übungs-IDs: Präfix = Seite (`do-und-does-…`), Diktat `<seite>-hoeren`, Nachsprechen `<seite>-nachsprechen`.

## Content structure

- Pfad: `src/<kapitel>/chapter.yaml`, Seiten `src/<kapitel>/<seite>.yaml`.
- Jede Seite hat dieselben Abschnitts-IDs in dieser Reihenfolge: `einstieg` (Szene der Figuren, erste leichte Aufgabe, „Das kannst du danach“), `neu` (Satzleiste, Bau-Karte, Merke-Kasten), `uebung` (mindestens vier Übungen, leicht → schwer), `anwenden` (`open-task` oder `speaking-task`), `weiter` (nächster Schritt an der Wand; am Kapitelende ein Rückblick). Titel sagen, was der Abschnitt tut. Die Wiederholungsseite hat nur Text und Tabelle.
- Länge: höchstens 350 Wörter Text, höchstens 4 Textblöcke hintereinander, Bild oder Übung in den ersten vier Blöcken. Jede Seite bringt einen neuen Schritt (`explainer-one-step`).
- Geschichte: Mr Hill hängt neben den Zeitstrahl der Klasse eine Satzleiste mit Karten an die Wand; Sophie, Ellie, Peter und Amir legen Sätze, fragen sich aus und schreiben Fragen für ein Klassenquiz. Figuren und Orte wie in #470 (nicht ändern): Sophie (blond, Zöpfe, grüne Jacke, aus Deutschland, wohnt bei den Parkers, 11 bis 12), Ellie Parker (11, roter Pferdeschwanz, rote Jacke), Peter Parker (9, kurze braune Haare, gelbe Jacke), Amir (11, schwarze Locken, Brille, blaue Jacke), Mr Hill (graue Haare, braune Jacke), Mrs Parker. Millbrook School, Schultag ab 8:45. Geburtstage: Peter 5. Mai, Ellie 10. Juli, Amir 12. Oktober, Sophie 14. Oktober. Tabellen heißen „Klassenzimmer-Poster · …“ und „Schulkalender · …“.
- Anrede „du“.
- **Stufe 9-10 (Kapitel 4, Konventionen Abschnitt 8):** Abschnitte `einstieg` (Vorwissen-Frage mit drei Optionen), `lesen` (Lesestück), `neu` (Regel an der Satzleiste), `uebung` (Verstehen, Belegen mit Zeile, Form, Diktat), `anwenden` (Nachsprechen, Schreibauftrag), `weiter`. Das Lesestück ist ein eigener Text (320 bis 380 Wörter) nach Fakten einer geöffneten Quelle, in drei Abschnitten A, B, C mit je einem Randglossar (`vocabulary`, Wörter über A1/A2) und einem Zahlenkasten (`table`, „… in Zahlen“) mit den Daten; unter dem Text steht die Quellenzeile. Keine Figuren, keine Szenen-SVG; das einzige Bild ist die Satzleiste. Hörsätze neu und kurz, nicht aus dem Lesestück kopiert. `punctuation: ok`, Anrede „du“.
- Figuren werden im Seitentext nicht vorgestellt: keine Altersangaben, keine Verwandtschaft, kein Datum, kein „wohnt bei der Familie Parker“. Die Startseite (`src/app.yaml`, `intro`) nennt sie nur mit Namen; eine Figur wird auf einer Seite nur benannt, wo die Aufgabe sie braucht. Wer wer ist, sagen nur die Bildunterschriften (Haare, Jacke).

## Terminology

- „Ausdruck“ (fester Ausdruck), nie „Wendung“. Fachbegriffe noun, verb, adjective, sentence, tense (aus #470); Zeitnamen wie in #472: simple present, simple past, Zeitstrahl, Punkt, Punktreihe, now.
- Neue Begriffe dieser App: **Satzleiste** (die Wand mit den Karten), **Satzkarte** (Subjekt, Verb, Objekt, Ort, Zeit, Fragewort, not), **Helfer** (do, does, did; Karte in Gelb), **Gepäck** (die Endung, die der Helfer trägt: „Der Helfer trägt das Gepäck, das Verb geht ohne.“), **Spiegel** (question tag am Satzende), **Kurzantwort**. Immer dieselben Wörter.
- Britisches Englisch (favourite, colour, football). Englische Aufgaben enthalten kein deutsches Wort. Englisches mit deutscher Bedeutung, wo ein Wort neu ist.
- Aussprache: keine Lesehilfe und keine Lautschrift hier (IPA gehört zu #482); Hörtexte nur als Sätze.

## Exercise patterns

Aufbau leicht → schwer: wählen/zuordnen/ordnen → Lücke → schreiben mit Cue → Korrektur → übersetzen/frei. Je Übung `mistakes` mit eigener Meldung und `hint`; gleichwertige Antworten mit `(a|b)` und `accepted`; Kurzformen (don't, doesn't, didn't, I'm not) zulassen.

- Karten ordnen: `ordering` mit Satzteilen (Stellung S – V – O – Ort – Zeit; Frage: Helfer – Subjekt – Verb).
- Helfer und Form wählen: `language-task` mode `choice` mit `distractors` (do/does/did; Verb mit oder ohne -s/-ed).
- Tabellen: mode `table` (Person ↔ Helfer ↔ Verb).
- Form bilden: mode `write` mit `cue` (`cue: "Peter · like · pizza"` → Does Peter like pizza?).
- Korrektur: Satz mit einem Fehler richtig schreiben.
- Zuordnen: `matching` (Frage ↔ Kurzantwort; Fragewort ↔ Antwort).
- Entscheiden mit Begründung: `single-choice`/`true-false`, die Rückmeldung nennt die Karte („Das Verb trägt kein Gepäck mehr“).
- Hören und schreiben: `language-task` mit `audio` (Diktat, je Seite höchstens drei ganze Sätze); Nachsprechen: `speaking-task`; freies Schreiben: `open-task`.
- Typische Fehler (jeweils `mistakes`): Does he plays; Do he play; Plays he; I not like (ohne do); Do you are (do bei be); Yes, I like. statt Yes, I do.; What does he plays; Where you live; Who does like pizza?; To who are you talking?; Did she played / Did she went; didn't + 2. Form; gleiche Polarität im question tag; falscher Helfer oder falsche Person im tag; Zeit vor Ort; Subjektkarte vergessen im Imperativ („You open“), Don't to run.
- Stufe 9-10 (Kapitel 4), Aufgaben in drei Stufen: Verstehen am Lesestück (`single-choice`, `true-false`, richtige Option nicht immer an erster Stelle), Belegen mit Zeile (`single-choice` mit Sätzen aus dem Text, gleichartige Optionen), Form (`language-task`: `choice` mit Distraktoren, `write` mit cue für Betonung beziehungsweise Umkehr, Korrektur; Diktat; Muster `emphase-widerspruch`: aus „didn't“ wird betontes did; `inversion-bilden`: normaler Satz → Umkehr). Typische Fehler: does/did + 3. Form oder 2. Form (She does makes, did won), Betonung ohne Helfer, Umkehr ohne Helfer (Never he has), Helfer und Verb doppelt (Not only did she sang), falscher Helfer (does statt did). `case: ok` bei der Betonung (Großbuchstaben).
- Keine Komponente (`prefer-built-in-block`); Ziehen von Karten wäre ein Wunsch für ein Inkrement.
- Keine Datendateien: jede Tatsache steht einmal in ihrer Seite.

## Figures

- **Satzleiste** (eine SVG-Familie `src/images/satzleiste-<seite>.svg`, eigene Zeichnung, `CC-BY-4.0`, gleich auf jeder Seite; Hintergrund #f4efe2, Schrift mindestens 16 im 480er viewBox): Karten Subjekt #2c6fd8, Verb #c0392b, Objekt #138d75, Ort #d35400, Zeit #8e44ad, Helfer #e6b800 (dunkle Schrift), not #7f8c8d, Fragewort #17a2b8, Präposition #6d4c41 (braun), Antwort (Yes/No) #5d6d7e. Aussage: Karten von links nach rechts S – V – O – Ort – Zeit. Frage: der Helfer springt (Bogen) vor das Subjekt, das Verb steht ohne Endung. Verneinung: not neben dem Helfer vor dem Verb. Subjektfrage: Subjektkarte wird zur Fragewortkarte, kein Helfer. Question tag: gestrichelte Linie als Spiegel am Satzende. In Aufgaben zeigt die Satzleiste nur die Legende, nie das Ergebnis.
- Skizzen der Familie: `.vibe/sketches/satzleiste-*.svg`.
- Gebaut (je eine Reihe oder mehrere Reihen untereinander): `satzleiste-aussage` (wortstellung), `-imperativ`, `-frage` (Aussage, Frage, Verneinung; do-und-does), `-kurzantworten`, `-fragewort`, `-subjektfrage`, `-praeposition`, `-did`, `-tag`, `-ganz` (Rückblick am Ende von question-tags, alle Plätze). Erzeugt mit einem Skript, das die Karten setzt (Kartenbreite folgt der Wortlänge, Beschriftung unter jeder Karte, Schrift 16 bis 17 im 480er viewBox); Kapitel 4: `satzleiste-emphase` (betonte Aussage, gelbe Helferkarte vor dem Verb) und `satzleiste-inversion` (der Helfer springt hinter das verneinende Wort); ein neues Bild ist eine neue Zeile in diesem Skript oder eine Kopie der SVG mit anderen Wörtern.
- Szenen (gebaut: `szene-wortstellung`, `-imperativ`, `-do-und-does`, `-kurzantworten`, `-fragewoerter`, `-subjektfragen`, `-praeposition-am-ende`, `-did`, `-question-tags`; Sprechblase zeigt nur die Frage, nie die Antwort): je Seite eine `szene-<seite>.svg` mit den Figuren, kopiert als `<g id>` aus `millbrook-klassenzimmer.svg` von #470 (hello-millbrook) und gleich gelassen; keine Fotos, keine Figuren aus Büchern, Filmen oder Marken. Quelle „eigene Zeichnung“, Lizenz `CC-BY-4.0`. `alt` sagt, was die Szene zeigt, nie die Lösung; die Bildunterschrift nennt, wer wer ist.
- Jede Figur funktioniert bei 360 px (viewBox, Beschriftung innerhalb).
- Poster mit Grammatik (Satzkarten, Helfer, Frage und Antwort) sind `table`-Blöcke. Die Tabelle „Klassenzimmer-Poster · Wörter dieser Seite“ ist ein Vokabelblock (`type: vocabulary`, `languages: { source: de, target: en }`, `entries` mit `target` und `source`; seit app-templates 0.14, mit Abdecken-Knöpfen): sie steht auf allen neun Seiten mit Übungen (nicht auf den Wiederholungsseiten). Neue Wörter einer Seite kommen als Eintrag dorthin; nur Vokabeln gehören in den Vokabelblock, Tabellen mit Bildung oder Regeln bleiben `table`.

## Sources

Karte `https://lernapps.net/apps/map/englisch.json`; Grundwortschatz `https://lernapps.net/apps/map/englisch/grundwortschatz/` (A1/A2; Wörter der Übungen stammen daraus; „does“ und „did“ sind Formen von do). Fakten aus Wikipedia (nur Fakten, keine Sätze, CC BY-SA): `Do-support` (do als Hilfsverb für Frage und Verneinung, wenn kein anderes Hilfsverb oder be da ist; danach die Grundform) und `Tag question` (Bildung und Gebrauch), geöffnet am 2026-11-21. Kapitel 4: Wikipedia (en) `Apollo 11` (Start 16. Juli und Landung 20. Juli 1969, Collins im Orbit, 216 Pfund Treibstoff, 25 Sekunden, 21,5 kg Mondmaterial, Mondspaziergang 2 h 31 min 40 s, 24. Juli Wasserung, rund 600 Millionen Zuschauer) und `Negative inversion` (Umkehr nach never und hardly; `not only` ist Grammatikwissen, dort nicht geprüft), geöffnet am 2026-11-24; Wikipedia (en) `Marie Curie` (Geburtsjahr, Umzug nach Paris, Nobelpreise 1903 und 1911, erste Professorin der Universität Paris 1906, Tod von Pierre 1906, `radioactivity` von ihr geprägt, Curie-Institut) und `Do-support` (betontes do), geöffnet am 2026-11-24; für `inversion` zusätzlich `Apollo 11` und `Subject–auxiliary inversion` (Daten und Regel, Stand siehe Seite). Das Lesestück ist ein eigener Text, keine Sätze der Quelle. Nicht geprüft: deutsche Wikipedia, Klexikon. Beispielsätze sind eigene aus dem Alltag der Figuren. Audio: KI-Stimme `bf_emma` (britisch, weiblich), mit Skill `lernapps-audio` erzeugt und als KI-generiert markiert. Material der Ersteller:in: keines.

## Adding a chapter or round

1. Baustein auf der Karte wählen (Kapitel 4: `emphase-do`, `inversion`, Stufe 9-10; keine erfundenen Kinder mehr, Beispiele aus Reden und Literatur, `explainer-age-appropriate`); die Voraussetzungen müssen auf früheren Seiten stehen oder eine Wiederholungsseite bekommen.
2. Seite `src/<kapitel>/<seite>.yaml` mit den Abschnitten `einstieg`, `neu`, `uebung`, `anwenden`, `weiter` anlegen, in `chapter.yaml` eintragen, Competency-ID setzen.
3. Satzleiste um den neuen Platz erweitern und das Poster um die Zeilen der Seite.
4. Übungen aus den Mustern oben, je mit `mistakes` und `hint`; 1 bis 3 ihrer Übungen in `selfAssessment` des Kapitels aufnehmen, wie Skill `lernapps-explainer-self-assessment` sagt (gebaut: je Seite `…-waehlen`/`…-bilden`, eine Übung ohne Bezug auf Tabelle oder Poster).
5. Hörtexte: Datei `src/audio/<satz>.mp3` und Eintrag in `.agents/skills/app-content/scripts/audio-texte.json` (Datei → Satz), erzeugt mit dem Skript `regen_audio.py` (aus hello-millbrook, schneidet das Ausklingen ab); Sätze nicht zwischen Seiten wiederholen, Namen am Satzende zweisilbig (Sophie, Peter, Ellie, Amir); anhören lassen.
6. Stufe 9-10: ein Lesestück (eigener Text nach Fakten einer geöffneten Quelle, 3 Abschnitte, Randglossar nach jedem Abschnitt, Zahlenkasten, Quellenzeile) vor der Regel; Fakten gegen die Quelle prüfen; keine Figuren.
7. Wörter gegen den Grundwortschatz prüfen; `npx --no -- lernapps check`; committen.

## Rules learned from mistakes

Aus #470 und #472 übernommen:
- Jede Übung fragt nur Wörter ab, die vorher auf der Seite stehen.
- Eine Tabelle, die eine Übung beantwortet, steht nicht direkt über ihr; die Antwort einer Frage steht nie im Absatz direkt darüber.
- Englische Aufgaben und Cues enthalten kein deutsches Wort.
- Mit `(a|b)` gleichwertige richtige Antworten zulassen; Kurzformen zulassen; `case: wrong` nur dort, wo die Seite Großschreibung unterrichtet.
- Audio: das Ausklingen der Stimme am Satzende abschneiden, Namen am Satzende zweisilbig.
- Audio: ein Hörsatz bleibt der natürliche Satz, ein Name am Ende nur als Anrede (Please listen, Amir.), nie wegen des Klangs; das Verb live am Satzende spricht die Stimme wie das Adjektiv („leive“): live nie ans Satzende, ein Name oder Wort dahinter (Where do Ellie and Amir live, Peter?).
- Bilder: Beschriftungen innerhalb des `viewBox`; die Bildunterschrift nennt, wer wer ist; das `alt` verrät nie die Lösung.
- Der Merke-Kasten nennt andere Verben als die Übungen, sonst schreiben die Kinder nur ab.
- Als Auswahl nur echte Lernerfehler, keine Unwörter.
- Hinweise und Meldungen der Selbsteinschätzung nennen weder „Spalte“ noch „Poster“ noch „oben“.
Aus dieser App (Lerner-Check der Musterseite, Sprachprüfung, Orchestrator-Prüfung):
- Keine Einführung der Figuren und keine Altersangaben in Seitentexten (Rückmeldung der Ersteller:in): kein Absatz „Wer legt die Karten?“, keine Vokabel „Mr Hill (der Englischlehrer)“.
- Die Auswahl der richtigen Antwort darf nicht an der Länge zu erkennen sein; Antwortsätze gleich lang und gleich konkret.
- Die Farben der Satzkarten sind nicht die Farben der Jacken der Kinder: der Text sagt es einmal.
- Ein Begriff (Subjekt, Verb, Objekt, not, they) steht auf der Seite, bevor eine Übung ihn braucht.
- „Wähle das richtige Wort“, nicht „den richtigen Helfer“, wo is/are als Distraktor stehen (be ist kein Helfer).
- Der Helfer wird auf der Seite des Imperativs (don't) zum ersten Mal gezeigt; spätere Seiten sagen „der gelbe Helfer, den du von don't kennst“.
- Tabellen-Übungen nehmen andere Verben und Personen als das Poster darüber.
- Keine `matching`-Aufgabe mit gleichen rechten Einträgen (Subjekt, Objekt): dort `multiple-choice`.
- Ein Satz auf zwei Absätze verteilt, höchstens drei neue Begriffe je Absatz; ein Merke-Kasten hat zwei bis drei Aussagen.
- Bei `accepted` mit `?` in der Flow-Liste den Eintrag in Anführungszeichen setzen.
- Offene Fehler der Vorlage `lernapps/app-templates` (dem Orchestrator gemeldet): `ordering` zeigt Auswahlfelder statt Karten; Tabellen-Übung bricht die Spalte „Person“ bei 360 px; Standardmeldung „Deine Fassung kann trotzdem richtig sein“ bei klar falschen Antworten; die Meldung zu Apostroph und Großschreibung nennt falsche Wörter.

## Hörliste

Hörsätze, die auf ein einsilbiges Wort enden und deshalb gezielt angehört werden sollen (Fehllaut am Ende möglich; das Ausklingen schneidet `regen_audio.py` ab). Satz und Datei in `src/audio/`:

- Amir didn't play football at school. (`amir-didnt-play-football-at-school.mp3`)
- Amir doesn't live here. (`amir-doesnt-live-here.mp3`)
- Amir plays football at school, doesn't he? (`amir-plays-football-at-school-doesnt-he.mp3`)
- Amir reads a book at home every day. (`amir-reads-a-book-at-home-every-day.mp3`)
- Do Ellie and Amir live here? (`do-ellie-and-amir-live-here.mp3`)
- Do Ellie and Peter like pizza? Yes, they do. (`do-ellie-and-peter-like-pizza-yes-they-do.mp3`)
- Do you eat pizza? Yes, I do. (`do-you-eat-pizza-yes-i-do.mp3`)
- Does Ellie play football? No, she doesn't. (`does-ellie-play-football-no-she-doesnt.mp3`)
- Does Mr Hill go home after school? (`does-mr-hill-go-home-after-school.mp3`)
- Does Sophie eat pizza? No, she doesn't. (`does-sophie-eat-pizza-no-she-doesnt.mp3`)
- Does Sophie study English at home? (`does-sophie-study-english-at-home.mp3`)
- Don't write here, please. (`dont-write-here-please.mp3`)
- Ellie and Peter play football in the park. (`ellie-and-peter-play-football-in-the-park.mp3`)
- Ellie eats pizza, doesn't she? (`ellie-eats-pizza-doesnt-she.mp3`)
- Is Ellie happy? Yes, she is. (`is-ellie-happy-yes-she-is.mp3`)
- Is Mr Hill happy? Yes, he is. (`is-mr-hill-happy-yes-he-is.mp3`)
- Mr Hill teaches English at school every day. (`mr-hill-teaches-english-at-school-every-day.mp3`)
- Peter doesn't eat pizza at school. (`peter-doesnt-eat-pizza-at-school.mp3`)
- Peter watched a film, didn't he? (`peter-watched-a-film-didnt-he.mp3`)
- Please read the book. (`please-read-the-book.mp3`)
- Read your book. (`read-your-book.mp3`)
- Sophie is happy, isn't she? (`sophie-is-happy-isnt-she.mp3`)
- Stand up and sit down. (`stand-up-and-sit-down.mp3`)
- What did Amir study after school? (`what-did-amir-study-after-school.mp3`)
- What did Sophie eat at home? (`what-did-sophie-eat-at-home.mp3`)
- What do you eat at school every day? (`what-do-you-eat-at-school-every-day.mp3`)
- What does Amir like at home? (`what-does-amir-like-at-home.mp3`)
- What does Mr Hill read at home? (`what-does-mr-hill-read-at-home.mp3`)
- What does Sophie eat at home? (`what-does-sophie-eat-at-home.mp3`)
- What does Sophie watch at school? (`what-does-sophie-watch-at-school.mp3`)
- When does Ellie read a book? (`when-does-ellie-read-a-book.mp3`)
- Where does Mr Hill come from? (`where-does-mr-hill-come-from.mp3`)
- Who do you eat lunch with? (`who-do-you-eat-lunch-with.mp3`)
- Who do you live with? (`who-do-you-live-with.mp3`)
- Who does Amir talk to at school? (`who-does-amir-talk-to-at-school.mp3`)
- Who does Ellie study with? (`who-does-ellie-study-with.mp3`)
- Who does Peter play with? (`who-does-peter-play-with.mp3`)
- Who likes pizza at school? (`who-likes-pizza-at-school.mp3`)
- You didn't eat lunch, did you? (`you-didnt-eat-lunch-did-you.mp3`)
- You don't like tea, do you? (`you-dont-like-tea-do-you.mp3`)

### Geschnittene Dateien (Fehllaut-Schnitt, `regen_audio.py` mit `valley_cut`, alle 54 Dateien neu erzeugt)

Der Trockenlauf (`DRY=1`, Ausgabe in ein Wegwerf-Verzeichnis) und der echte Lauf melden dieselben vier Schnitte:

- Is Mr Hill happy? Yes, he is. (`is-mr-hill-happy-yes-he-is.mp3`): bei 1935 ms, 95 ms entfernt (4,7 %)
- Is Ellie happy? Yes, she is. (`is-ellie-happy-yes-she-is.mp3`): bei 1515 ms, 85 ms entfernt (5,3 %)
- When does Ellie read a book? (`when-does-ellie-read-a-book.mp3`): bei 1335 ms, 25 ms entfernt (1,8 %)
- Please read the book. (`please-read-the-book.mp3`): bei 1205 ms, 25 ms entfernt (2,0 %)

### Neue Hörsätze Kapitel 4 (Seite `emphase-do`)

Enden auf ein einsilbiges Wort, gezielt anhören: She did love her work. (`she-did-love-her-work.mp3`) · Critics do forget one thing. (`critics-do-forget-one-thing.mp3`) · He did say that. (`he-did-say-that.mp3`, Fehllaut-Schnitt 25 ms) · I do think she deserved it. (`i-do-think-she-deserved-it.mp3`, Fehllaut-Schnitt 45 ms). Mehrsilbiges Ende: We do need more stories like hers. · She did change science.

### Neue Hörsätze Kapitel 4 (Seite `inversion`)

Enden auf ein einsilbiges Wort, gezielt anhören: Never have I felt so tired. (`never-have-i-felt-so-tired.mp3`, Fehllaut-Schnitt 25 ms) · Hardly had she left when it rained. (`hardly-had-she-left-when-it-rained.mp3`) · Not only did he come, but he stayed. (`not-only-did-he-come-but-he-stayed.mp3`). Mehrsilbiges Ende: Seldom does he speak in public. · Never before had I seen the sea. · Seldom do we hear such a story. (Risiko: eine Silbe wird angeschnitten)

Gezielt anhören, auch wenn nichts geschnitten wurde: Do you play football every Saturday? · Do Ellie and Amir play football? · Sophie reads a book at home on Monday. · Where does Amir play football on Sunday? · Why does Peter like football? · Who eats lunch with Ellie? · Who lives with Sophie? · Did Peter eat pizza at school yesterday? · Sophie didn't watch a film yesterday. · Did Ellie and Peter go home yesterday? · Ellie plays football at school on Friday. · Peter eats pizza in the park on Sunday. · Please listen, Amir. · Sit down and listen.
