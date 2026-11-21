---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

„Sätze bauen: Aussage, Frage und Verneinung mit do“: Explainer (Strang-App `englisch/grammatik`, Format 2, Sprache Deutsch, englische Beispiele) über Wortstellung, Imperativ, Fragen, Verneinung mit dem Helfer do, Kurzantworten und question tags. Auftrag: Issue lernapps/apps#473 (Epic lernapps/apps#489, Konventionen dort). Die erste Version baut nur Stufe 5-6 (Kapitel 1 bis 3); Kapitel 4 „Betonen und umstellen“ (Stufe 9-10: `emphase-do`, `inversion`) kommt als Inkrement `increment/<NN>-<name>`.

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

Die „Ich kann“-Sätze stehen in `src/<kapitel>/<seite>.yaml` wie in der Karte (nicht umformulieren). Übungs-IDs: Präfix = Seite (`do-und-does-…`), Diktat `<seite>-hoeren`, Nachsprechen `<seite>-nachsprechen`.

## Content structure

- Pfad: `src/<kapitel>/chapter.yaml`, Seiten `src/<kapitel>/<seite>.yaml`.
- Jede Seite hat dieselben Abschnitts-IDs in dieser Reihenfolge: `einstieg` (Szene der Figuren, erste leichte Aufgabe, „Das kannst du danach“), `neu` (Satzleiste, Bau-Karte, Merke-Kasten), `uebung` (mindestens vier Übungen, leicht → schwer), `anwenden` (`open-task` oder `speaking-task`), `weiter` (nächster Schritt an der Wand; am Kapitelende ein Rückblick). Titel sagen, was der Abschnitt tut. Die Wiederholungsseite hat nur Text und Tabelle.
- Länge: höchstens 350 Wörter Text, höchstens 4 Textblöcke hintereinander, Bild oder Übung in den ersten vier Blöcken. Jede Seite bringt einen neuen Schritt (`explainer-one-step`).
- Geschichte: Mr Hill hängt neben den Zeitstrahl der Klasse eine Satzleiste mit Karten an die Wand; Sophie, Ellie, Peter und Amir legen Sätze, fragen sich aus und schreiben Fragen für ein Klassenquiz. Figuren und Orte wie in #470 (nicht ändern): Sophie (blond, Zöpfe, grüne Jacke, aus Deutschland, wohnt bei den Parkers, 11 bis 12), Ellie Parker (11, roter Pferdeschwanz, rote Jacke), Peter Parker (9, kurze braune Haare, gelbe Jacke), Amir (11, schwarze Locken, Brille, blaue Jacke), Mr Hill (graue Haare, braune Jacke), Mrs Parker. Millbrook School, Schultag ab 8:45. Geburtstage: Peter 5. Mai, Ellie 10. Juli, Amir 12. Oktober, Sophie 14. Oktober. Tabellen heißen „Klassenzimmer-Poster · …“ und „Schulkalender · …“.
- Anrede „du“.

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
- Keine Komponente (`prefer-built-in-block`); Ziehen von Karten wäre ein Wunsch für ein Inkrement.
- Keine Datendateien: jede Tatsache steht einmal in ihrer Seite.

## Figures

- **Satzleiste** (eine SVG-Familie `src/images/satzleiste-<seite>.svg`, eigene Zeichnung, `CC-BY-4.0`, gleich auf jeder Seite; Hintergrund #f4efe2, Schrift mindestens 16 im 480er viewBox): Karten Subjekt #2c6fd8, Verb #c0392b, Objekt #138d75, Ort #d35400, Zeit #8e44ad, Helfer #e6b800 (dunkle Schrift), not #7f8c8d, Fragewort #17a2b8. Aussage: Karten von links nach rechts S – V – O – Ort – Zeit. Frage: der Helfer springt (Bogen) vor das Subjekt, das Verb steht ohne Endung. Verneinung: not neben dem Helfer vor dem Verb. Subjektfrage: Subjektkarte wird zur Fragewortkarte, kein Helfer. Question tag: gestrichelte Linie als Spiegel am Satzende. In Aufgaben zeigt die Satzleiste nur die Legende, nie das Ergebnis.
- Skizzen der Familie: `.vibe/sketches/satzleiste-*.svg`.
- Gebaut (je eine Reihe oder mehrere Reihen untereinander): `satzleiste-aussage` (wortstellung), `-imperativ`, `-frage` (Aussage, Frage, Verneinung; do-und-does), `-kurzantworten`, `-fragewort`, `-subjektfrage`, `-praeposition`, `-did`, `-tag`, `-ganz` (Rückblick am Ende von question-tags, alle Plätze). Erzeugt mit einem Skript, das die Karten setzt (Kartenbreite folgt der Wortlänge, Beschriftung unter jeder Karte, Schrift 16 bis 17 im 480er viewBox); ein neues Bild ist eine neue Zeile in diesem Skript oder eine Kopie der SVG mit anderen Wörtern.
- Szenen (gebaut: `szene-wortstellung`, `-imperativ`, `-do-und-does`, `-kurzantworten`, `-fragewoerter`, `-subjektfragen`, `-praeposition-am-ende`, `-did`, `-question-tags`; Sprechblase zeigt nur die Frage, nie die Antwort): je Seite eine `szene-<seite>.svg` mit den Figuren, kopiert als `<g id>` aus `millbrook-klassenzimmer.svg` von #470 (hello-millbrook) und gleich gelassen; keine Fotos, keine Figuren aus Büchern, Filmen oder Marken. Quelle „eigene Zeichnung“, Lizenz `CC-BY-4.0`. `alt` sagt, was die Szene zeigt, nie die Lösung; die Bildunterschrift nennt, wer wer ist.
- Jede Figur funktioniert bei 360 px (viewBox, Beschriftung innerhalb).
- Poster sind `table`-Blöcke, wachsen von Seite zu Seite.

## Sources

Karte `https://lernapps.net/apps/map/englisch.json`; Grundwortschatz `https://lernapps.net/apps/map/englisch/grundwortschatz/` (A1/A2; Wörter der Übungen stammen daraus; „does“ und „did“ sind Formen von do). Fakten aus Wikipedia (nur Fakten, keine Sätze, CC BY-SA): `Do-support` (do als Hilfsverb für Frage und Verneinung, wenn kein anderes Hilfsverb oder be da ist; danach die Grundform) und `Tag question` (Bildung und Gebrauch), geöffnet am 2026-11-21. Nicht geprüft: deutsche Wikipedia, Klexikon. Beispielsätze sind eigene aus dem Alltag der Figuren. Audio: KI-Stimme `bf_emma` (britisch, weiblich), mit Skill `lernapps-audio` erzeugt und als KI-generiert markiert. Material der Ersteller:in: keines.

## Adding a chapter or round

1. Baustein auf der Karte wählen (Kapitel 4: `emphase-do`, `inversion`, Stufe 9-10; keine erfundenen Kinder mehr, Beispiele aus Reden und Literatur, `explainer-age-appropriate`); die Voraussetzungen müssen auf früheren Seiten stehen oder eine Wiederholungsseite bekommen.
2. Seite `src/<kapitel>/<seite>.yaml` mit den Abschnitten `einstieg`, `neu`, `uebung`, `anwenden`, `weiter` anlegen, in `chapter.yaml` eintragen, Competency-ID setzen.
3. Satzleiste um den neuen Platz erweitern und das Poster um die Zeilen der Seite.
4. Übungen aus den Mustern oben, je mit `mistakes` und `hint`; 1 bis 3 ihrer Übungen in `selfAssessment` des Kapitels aufnehmen, wie Skill `lernapps-explainer-self-assessment` sagt (gebaut: je Seite `…-waehlen`/`…-bilden`, eine Übung ohne Bezug auf Tabelle oder Poster).
5. Hörtexte: Datei `src/audio/<satz>.mp3` und Eintrag in `.agents/skills/app-content/scripts/audio-texte.json` (Datei → Satz), erzeugt mit dem Skript `regen_audio.py` (aus hello-millbrook, schneidet das Ausklingen ab); Sätze nicht zwischen Seiten wiederholen, Namen am Satzende zweisilbig (Sophie, Peter, Ellie, Amir); anhören lassen.
6. Wörter gegen den Grundwortschatz prüfen; `npx --no -- lernapps check`; committen.

## Rules learned from mistakes

Aus #470 und #472 übernommen:
- Jede Übung fragt nur Wörter ab, die vorher auf der Seite stehen.
- Eine Tabelle, die eine Übung beantwortet, steht nicht direkt über ihr; die Antwort einer Frage steht nie im Absatz direkt darüber.
- Englische Aufgaben und Cues enthalten kein deutsches Wort.
- Mit `(a|b)` gleichwertige richtige Antworten zulassen; Kurzformen zulassen; `case: wrong` nur dort, wo die Seite Großschreibung unterrichtet.
- Audio: das Ausklingen der Stimme am Satzende abschneiden, Namen am Satzende zweisilbig.
- Bilder: Beschriftungen innerhalb des `viewBox`; die Bildunterschrift nennt, wer wer ist; das `alt` verrät nie die Lösung.
- Der Merke-Kasten nennt andere Verben als die Übungen, sonst schreiben die Kinder nur ab.
- Als Auswahl nur echte Lernerfehler, keine Unwörter.
- Hinweise und Meldungen der Selbsteinschätzung nennen weder „Spalte“ noch „Poster“ noch „oben“.
Aus dieser App (Lerner-Check der Musterseite, Sprachprüfung, Orchestrator-Prüfung):
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
