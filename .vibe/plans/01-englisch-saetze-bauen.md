---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Written by `lernapps plan` and the hooks. Never change a key or a value by hand.
# Archetype, null until chosen in Explore. Allowed values: explainer, interactive, quiz.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit.
phase: code
# prePushFailures: failed pre-push runs, written by the hook.
prePushFailures: 0
# failedChecks: failed rules and runs, written by lernapps check and the hooks.
failedChecks: {}
---

# Plan: englisch-saetze-bauen, first version

<!--
For you, the assistant. The process is in AGENTS.md; this plan holds the method.
- `npx --no -- lernapps plan next` prints the task to do now, `plan done` ticks it and prints the next one.
- You write only below Goal, Key decisions, Notes, Answers, Entry draft, Content method and Retrospective, in the
  creator's language. Delete the comment of a section once the section is filled.
- Work on the branch `work`, locally: push nothing before Commit.
-->

*Started 2026-11-21. Explore, Plan, Code, Commit.*

## Goal

<!-- 1–2 sentences: what learners do, what they learn. -->

## Key decisions

- Archetyp `explainer`: Lernende lesen Seiten mit Erklärung und üben je Seite; so sind Format 2 und das Issue vorgegeben. `quiz` (keine Erklärseiten) und `interactive` (Spiel, Zeitdruck) passen nicht. Der Explainer kann Text, Tabellen, Bilder, Übungen, Sprachaufgaben mit Audio; er kann kein Spiel und keinen Sprachvergleich (niemand bewertet das Sprechen), kein Ziehen von Karten ohne Komponente (die Satzkarten sind Bilder und `ordering`).

## Notes

Karte (Englisch, `https://lernapps.net/apps/map/englisch.json`) gelesen, Fokus `competency`. Der Auftrag (Issue #473) bringt den Inhalt: die neun Bausteine der Stufe 5-6 sind alle Lücken (`practisedBy` leer): `wortstellung` (Schritt 1), `imperativ` (2), `simple-present-fragen` (3, öffnet 21), `kurzantworten` (4), `fragewoerter` (4, öffnet 10), `simple-past-fragen` (4), `subjektfragen` (5), `fragen-praeposition-ende` (5), `question-tags` (5). Von außen gebraucht (je eine Wiederholungsseite `recap`): `classroom-phrases` (#470, für `imperativ`), `simple-present` und `to-be` (#472, für `simple-present-fragen`, `kurzantworten`), `simple-past` (#472, für `simple-past-fragen`).
**Strang und Kapitel:** Strang-App `englisch/grammatik` (Format 2), nur Stufe 5-6. Kapitel und Seiten (Datei `<kapitel>/<seite>`):
1. `aussage-und-aufforderung` „Aussage und Aufforderung“: Sammel-Wiederholung `recap: englisch/classroom-phrases` (`das-brauchst-du`, ohne Übung), `wortstellung` → `wortstellung`, `imperativ` → `imperativ` (hier tritt don't als erster Helfer auf).
2. `fragen-mit-do` „Fragen und verneinen mit do“: Sammel-Wiederholung `[englisch/simple-present, englisch/to-be]` (`das-brauchst-du`), `simple-present-fragen` → `do-und-does`, `kurzantworten` → `kurzantworten`, `fragewoerter` → `fragewoerter`, `subjektfragen` → `subjektfragen`, `fragen-praeposition-ende` → `praeposition-am-ende`.
3. `did-und-tags` „did und question tags“: Wiederholung `englisch/simple-past` (`das-brauchst-du`), `simple-past-fragen` → `did`, `question-tags` → `question-tags`.
Ordnung nach `requires`: kurzantworten braucht `to-be` und `simple-present-fragen`; question-tags braucht `to-be` und `simple-past-fragen` (to-be steht in Kapitel 2 als Wiederholung). Kapitel 4 (`emphase-do`, `inversion`, Stufe 9-10) kommt als Inkrement.
**Das eine wachsende Bild:** die Satzkarten (Subjekt, Verb, Objekt, Ort, Zeit; Helfer do/does/did als eigene Karte), die Satzleiste wie der Zeitstrahl in #472. Der Helfer springt vor das Subjekt (Frage) oder mit not vor das Verb (Verneinung) und nimmt dem Verb die Endung ab (does + Grundform, did + Grundform): „Der Helfer trägt das Gepäck, das Verb geht ohne.“
**Wie die Lernenden dahin kommen (ein Satz je Baustein, Fehler, die die Rückmeldung fängt):**
- `wortstellung`: Sie legen Karten in die Reihenfolge S – V – O – Ort – Zeit (`ordering`) und lesen sie an Beispielen ab. Fehler: Zeit vor Ort („I play football on Saturday at school“ statt „at school on Saturday“), Verb vor Subjekt, Objekt zwischen Subjekt und Verb („I football play“).
- `imperativ`: Aus dem Satz ohne Subjektkarte („You open the door“ → „Open the door“) und mit don't davor. Fehler: „You open“, „Not run“, „Don't to run“.
- `simple-present-fragen`: Sie setzen den Helfer ab und tauschen ihn vor die Subjektkarte; das Verb verliert das -s (does he play). Fehler: „Does he plays“, „Do he play“, „Plays he“, Verneinung ohne do („I not like“), do bei be („Do you are“).
- `kurzantworten`: Nur der Helfer wird wiederholt (Yes, I do. / No, she doesn't. / Yes, I am). Fehler: „Yes, I like.“, „Yes, I do like.“, do statt be.
- `fragewoerter`: Fragewort – Helfer – Subjekt – Verb; wählen und ordnen. Fehler: „Where you live“, „What does he plays“, who/whose, when/where.
- `subjektfragen`: Fragt man nach dem Subjekt, bleibt der Helfer weg, die Subjektkarte wird zum Fragewort (Who likes pizza?). Fehler: „Who does like pizza?“, Objektfrage ohne Helfer.
- `fragen-praeposition-ende`: Die Präposition bleibt am Ende (Who are you talking to?). Fehler: „To who are you talking?“ (die deutsche Stellung „Mit wem sprichst du?“ als Vorbild); die Rückmeldung nennt den Unterschied zum Deutschen und sagt, dass förmliches „To whom …“ selten ist.
- `simple-past-fragen`: Der Helfer geht in die Vergangenheit, did trägt das -ed (Did she play?, nicht „Did she played“). Fehler: „Did she played“, „Did she went“, didn't + 2. Form.
- `question-tags`: Aus positiv wird negativ und umgekehrt, der Helfer kommt zurück (You like it, don't you?; She is tired, isn't she?). Fehler: gleiche Polarität, falscher Helfer, falsche Person im Tag.
**Quellen (geöffnet am 2026-11-21, nur Fakten):** Wikipedia (en) „Do-support“ (do als Hilfsverb für Frage und Verneinung, wenn kein anderes Hilfsverb oder be da ist; danach steht die Grundform ohne Endung; do auch zur Betonung → Kapitel 4) und „Tag question“ (Bildung und Gebrauch von question tags); Lernlandkarte Englisch (Bausteine, `requires`); Grundwortschatz Englisch (A1/A2: do, question, answer, who, what, where, when, why, how, whose, often, always, never, yesterday, tomorrow, pizza, cake gefunden; „does“ und „did“ sind Formen von do). Nicht geprüft: deutsche Wikipedia und Klexikon (kein Artikel nötig), „English auxiliary verbs“ nur überflogen. Beispielsätze sind eigene aus dem Alltag der Figuren. Fehlende Bausteine der Karte: keine bemerkt.
**Umfang:** In: die neun Bausteine der Stufe 5-6 in drei Kapiteln; Fragen und Verneinung im simple present (do, does, don't, doesn't) und simple past (did, didn't), be wird nur wiederholt (be braucht kein do), Imperativ mit don't, Kurzantworten, die sieben Fragewörter who, what, where, when, why, how, whose, Subjekt- und Objektfragen, Präposition am Ende, question tags mit be, do und did (Beispiele nur mit Verben aus A1/A2). Nicht in diesem Stand und warum: Betonung mit do und Inversion (Kapitel 4, Stufe 9-10, Inkrement), Modalverben und andere Hilfsverben in Fragen und question tags (kein Baustein dieser Stufe), Nebensätze, indirekte Rede und indirekte Fragen (#481), Satzmelodie der Frage (#482), Stellung der Adverbien (#476). Zeiten selbst stehen in #472 und werden nur wiederholt. Datenumfang: simple present und simple past, alle Personen (ich bis sie), Verben aus A1/A2; regelmäßige und die 38 unregelmäßigen Verben aus #472 für did. Sprache: Deutsch (Erklärung), englische Beispiele, britisches Englisch, `languages: [de]`. Audio (Stimme `bf_emma`): Diktat und Nachsprechen, je Seite höchstens sechs ganze Sätze, Namen am Satzende zweisilbig.
**Seitendateien (zur Klarheit, die Code-Aufgaben nennen sie wegen eines Schreibfehlers beim Anlegen nur teilweise):** `aussage-und-aufforderung/{das-brauchst-du,wortstellung,imperativ}`, `fragen-mit-do/{das-brauchst-du,do-und-does,kurzantworten,fragewoerter,subjektfragen,praeposition-am-ende}`, `did-und-tags/{das-brauchst-du,did,question-tags}`; Bilder `satzleiste-{aussage,imperativ,frage,verneinung,kurzantworten,fragewort,subjektfrage,praeposition,did,tag,ganz}.svg`, Szenen `szene-<seite>.svg`.
Übungsmuster (Referenz Fremdsprachen): Reihe ordnen (`ordering`, Satzkarten), Form wählen (`language-task` choice mit `distractors`), Form bilden (write mit `cue`), Lücke (`gap`), Entscheiden mit Begründung, Diktat und Nachsprechen (Audio, `bf_emma`), freies Schreiben (`open-task`).

## Explore

<!--
- Find out what the app teaches, for whom, how much and how it looks. Ask; write no code, run no `create`.
- An answer counts only in the creator's words under "Answers". At most 2 questions per message, one topic each.
-->

### Tasks

- [x] Check the start: the folder `.agents/skills/lernapps-app` exists (else stop and tell the creator that the folder
      was not started with `init`), and `git branch --show-current` prints `work` (else `git switch -c work`).
- [x] Load skill `lernapps-app`. Tell the creator in two sentences what a lernapps app is and where it will live: at
      their own address, free and public, and once listed as a copy on lernapps.net. Say that the technical part
      (GitHub) comes at the end and that you do it.
- [x] Interview: ask the topics "Goal" and "Learners" of "Answers".
- [x] Load skill `lernapps-map-assignment` and read the learning map of the subject as it says. The creator brings
      the content themselves (material, a word list, the pages): note under "Notes" which competencies of the map it
      covers. Else write the skill's assignment, with its story; the creator's yes answers the topics Content and
      Amount. A subject without a map: skip this task and say so.
- [x] Load skill `lernapps-exercise-patterns` and read its reference for the subject. Note under "Notes" how learners
      will practise what the goal names.
- [x] Choose the archetype as skill `lernapps-app` says: read the README of each archetype in question, then tell the
      creator in plain words what the chosen one can and cannot do. Write the archetype and its reason under "Key
      decisions".
- [x] Run `npx --no -- lernapps skills --archetype <name>` with the chosen archetype. It installs the archetype's
      skills and adds the archetype's tasks to this plan.
- [x] Load skill `lernapps-explainer-design`. An explainer has the look of the runtime: write "fixed by the
      archetype" under the topic "Look and feel" of "Answers".
- [x] Interview: ask every other topic of "Answers", in order. Leave out only a topic that an answer of the creator
      already covers, and note which answer. A topic nobody answered is asked once before you write an assumption
      with "(guess)".
- [x] Load skill `lernapps-content-research` and research as it says. Write under "Notes": the strand or subject, the
      competencies by chapter with their ids, the sources you opened.
- [x] Write under "Notes" which competency goes on which page and which pages form a chapter, as "Map the content" of
      skill `lernapps-explainer-design` says. Per page, name the prerequisites the app does not practise.
- [x] Write under "Notes", one line per competency: how learners get there (they derive it, they do not only read it
      off), and which misconception the feedback catches.
- [x] Write under "Notes" the scope: what is in, what is out and why, the data range (for example "all main-group
      elements", never a silent "1–20"), the languages.
- [x] **Checkpoint:** research. Show in plain words: the strand or why none, the competencies by chapter, the didactic
      approach, the scope, every "(guess)", the sources and what is unchecked, the archetype and its reason. Stop and
      wait. Changes: change them, then ask again.
      Creator: Ja, du darfst zum Plan übergehen. 9 Bausteine = 9 Seiten + 3 Wiederholungsseiten = 12 Seiten.

### Answers

<!-- The interview: per topic the creator's answer, in their words. Keep the topics. -->

- Goal: "Ja", Satzkarten, Helfer do/does/did, Kurzantworten, Fragewörter, Subjektfragen, did und question tags (Stufe 5-6): Lernende bauen englische Sätze aus farbigen Satzkarten (Subjekt, Verb, Objekt, Ort, Zeit) und verwandeln sie mit dem Helfer in Fragen und Verneinungen; sie verstehen, warum Englisch dafür ein Hilfsverb braucht.
- Learners: "Ja", Englisch Klasse 5-6, Anfänger A1/A2, kennen Sophie, Ellie, Peter, Amir aus Hello, Millbrook und die Zeiten aus #472 (Zeitstrahl, simple present, simple past). Archetyp `explainer`: Ja.
- Model and focus: die fertigen Pull-Requests `lernapps/englisch-pronomen`, `englisch-zeiten`, `englisch-verbketten` (Übungen und das eine wachsende Bild); kein Spiel.
- Hurdles: typische Fehler selbst aus den Seiten der Reihe und dem Issue (kein do bei be, do + 3. Person -s, did + 2. Form, Wortstellung der Fragewörter, Verneinung ohne do).
- Content: ich schreibe ihn aus dem Issue, kein eigenes Material.
- Amount: Kapitel 1 bis 3 (Stufe 5-6), Kapitel 4 später als Inkrement.
- Languages: Deutsch (Erklärung) mit englischen Beispielen.
- Look and feel: fixed by the archetype (von der Runtime vorgegeben, ruhig wie ein Arbeitsblatt).
- Terms: „Ausdruck“, „Klassenzimmer-Poster“, „Schulkalender“; Satzkarten und der Helfer do als eigene Begriffe aus dem Issue.
- Finding the app: (guess), wie sonst.

## Plan

<!--
- Map the confirmed content onto the archetype. No new content questions: a gap in the content goes back to Explore.
- The creator confirms the plan in one read. After the yes you work on your own.
-->

### Tasks

- [x] Map the content as "Map the content" of skill `lernapps-explainer-design` says, and write the result under
      "Content method".
- [x] Choose a pattern per competency as skill `lernapps-exercise-patterns` says, and add it to "Content method".
- [x] Add to "Content method" one line per page, as "Engagement" of skill `lernapps-explainer-design` says: the
      opening task, the change of activity, the reward, the story.
- [x] Add the tasks of Code, each one a piece of work that ends in a commit. First the pattern: one complete page or
      screen, `npx --no -- lernapps plan add --at pattern "<task>"`. Then the others, one call each:
      `npx --no -- lernapps plan add --at pages "<task>"`. Each task says what it builds and what it shows.
- [x] Draw a sketch of each screen, component or interactive exercise: a static SVG or image, or the steps with what
      learners see after each. Keep the files in `.vibe/sketches/`.
- [x] Show the creator, short: goal, competencies by chapter, the Code tasks, the sketches, and the content method in
      plain words (what learners see and do, what the app cannot do). At most 2 questions.
- [x] **Checkpoint:** confirm the plan and the content method. Stop and wait for an explicit yes. Changes: change
      them, then ask again.
      Creator: Ja, Gesamtplan ok. Ja, do-und-does als Musterseite. Bedingungen: competencies je Seite auf Karten-Ids, Zeitstrahl-Begriffe aus #472 unverändert, vor Musterseite Lerner-Check und Sprachprüfung mit Sub-Agent.

### Content method

**Quelle der Wörter:** Grundwortschatz Englisch (https://lernapps.net/apps/map/englisch/grundwortschatz/), A1 und A2; außerhalb der Liste nur, was eine Situation braucht und die Seite erklärt (Satzkarte, Helfer, question tag werden als Begriffe erklärt). Wörter der Übungen stehen vorher auf der Seite (Poster „Wörter dieser Seite“). Anschluss an #472 (`lernapps/englisch-zeiten`, `work`): gleiche Figuren, gleiche Begriffe (Poster, Schulkalender, Ausdruck, simple present, simple past, Zeitstrahl für die Zeiten), die Satzleiste ist das neue, eine Seite lang wachsende Bild.
**Geschichte:** Mr Hill hängt neben den Zeitstrahl eine Satzleiste mit Karten an die Wand (Millbrook School). Sophie, Ellie, Peter und Amir legen Sätze mit Karten, fragen sich gegenseitig aus und schreiben Fragen für ein Quiz. Figuren und Orte wie in #470 und #472, gezeichnet je Seite als Szene (`szene-<seite>.svg`, `<g id>` kopiert aus `millbrook-klassenzimmer.svg` von hello-millbrook).
**Das wachsende Bild: die Satzleiste** (eine SVG-Familie `src/images/satzleiste-<seite>.svg`, eigene Zeichnung, CC-BY-4.0, gleiche Farben auf jeder Seite; Hintergrund wie der Zeitstrahl, Schrift mindestens 16 im 480er viewBox). Karten: Subjekt (blau), Verb (rot), Objekt (grün), Ort (orange), Zeit (violett), Helfer do/does/did (gelb, mit kleinem Gepäck-Zeichen), not (grau), Fragewort (türkis). Aussage = Karten von links nach rechts S – V – O – Ort – Zeit; Frage = Helfer springt vor S (Pfeil), das Verb steht danach ohne Endung; Verneinung = not neben dem Helfer vor dem Verb; Subjektfrage = die Subjektkarte wird zur Fragewortkarte, kein Helfer; question tag = Spiegel am Satzende (Farbwechsel positiv/negativ). In Aufgaben zeigt das Bild nur die Legende, nie das Ergebnis.
**Je Seite dieselben Abschnitte** (wie #472): `einstieg` (Szene, erste leichte Aufgabe, „Das kannst du danach“), `neu` (Satzleiste, Bau-Karte, Merke), `uebung` (mindestens vier, leicht → schwer), `anwenden` (`open-task` oder `speaking-task`), `weiter`. Wiederholungsseiten (`das-brauchst-du`): nur Text und Tabelle (Poster), kein Bild nötig außer wo es hilft, keine Übung, `recap` nennt die Bausteine.
**Engagement je Seite (Opening / Change / Reward / Story / Repeat):**
- `das-brauchst-du` K1: Ausdrücke vom Poster (Open the door. Sit down.) als bekannte Befehle; keine Übung; Story: Mr Hill gibt Anweisungen, die Kinder legen sie als Karten.
- `wortstellung`: Opening: Sophies Satz ist durcheinander, Reihenfolge wählen; dann Karten ordnen (`ordering`), Ort-vor-Zeit-Regel, Satz bauen, Karte für die Satzleiste schreiben; Reward: ein eigener Satz hängt an der Satzleiste.
- `imperativ`: Opening: Mr Hill sagt „Open the door.“ (wer ist das Subjekt?); Subjektkarte fällt weg; don't als erster Helfer; Sätze vom Poster mit Regel.
- `das-brauchst-du` K2: simple present (-s bei he/she/it) und to-be (am/is/are) als Poster-Tabelle, kein Übungsteil.
- `do-und-does` (Musterseite): Opening: Ellie fragt „Does Peter like pizza?“ und Sophie sieht die Karte springen; Satzleiste: Helfer springt nach vorn, Verb ohne -s; Verneinung mit not; Übungen: wählen, ordnen, bilden mit cue, Korrektur, übersetzen, Diktat; Reward: Fragen für das Klassenquiz.
- `kurzantworten`: Opening: Ja-Nein-Frage, welche Antwort passt; nur der Helfer wird wiederholt; do bei Frage mit do, am/is/are bei Frage mit be; Kurzantworten zuordnen, schreiben, nachsprechen.
- `fragewoerter`: Fragewort vor den Helfer; sieben Fragewörter zuordnen, Fragen ordnen und bilden; Quiz-Karten schreiben.
- `subjektfragen`: Opening: Who likes pizza? gegen Who does Peter like?; die Subjektkarte wird zur Frage; unterscheiden und bilden.
- `praeposition-am-ende`: Opening: Who are you talking to?; Präposition bleibt am Ende, mit dem Deutschen verglichen (Mit wem sprichst du?); ordnen und bilden.
- `das-brauchst-du` K3: simple past (-ed und die 38 unregelmäßigen Verben aus #472 nur als Verweis, nicht wiederholt); Zeitstrahl-Punkt mit Zeitangabe.
- `did`: Opening: Did Peter play football yesterday?; did trägt das -ed, das Verb geht ohne („der Helfer trägt das Gepäck“); didn't; Fehler „Did she went“; Frage in der Vergangenheit mit Fragewort.
- `question-tags`: Opening: „You like it, don't you?“; der Spiegel am Satzende; positiv ↔ negativ; Helfer mit be, do, does, did; wählen, bilden, Diktat. Rückblick: alle Kartenplätze auf einer Satzleiste (`satzleiste-ganz.svg`).
Repeat nur mit Absicht: dieselbe Regel in anderem Gewand (Karte, Tabelle, Satz), nicht dieselben Sätze.

**Muster je Baustein** (Kind der Kompetenz → Muster; Beispiel):
- Wortstellung, Imperativ → ordnen (`ordering` mit Satzteilen), `choice` mit Distraktoren; Beispiel: park · play · in the · football · on Saturday → „I play football in the park on Saturday.“
- Fragen und Verneinen (simple present, simple past) → Form bilden (`language-task` `write` mit `cue`), Korrektur („Does she plays …“), `choice` mit Distraktoren, `table` (Person ↔ Helfer ↔ Verb), Übersetzen; Beispiel: cue „Peter · like · pizza“ → „Does Peter like pizza?“.
- Kurzantworten → Zuordnen (`matching` Frage ↔ Kurzantwort), `gap`, `write`.
- Fragewörter → zuordnen (Fragewort ↔ Antwort), ordnen, bilden.
- Subjekt-/Objektfragen → entscheiden (`choice`) mit Begründung in der Rückmeldung, bilden.
- Präposition am Ende → ordnen und bilden, übersetzen.
- Question tags → `choice`/`gap` mit Distraktoren, `write` mit cue („Ellie plays football“ → „, doesn't she?“).
- Alle Seiten: Diktat (`language-task` mit `audio`, höchstens drei ganze Sätze) und Nachsprechen (`speaking-task`, drei Sätze); freies Schreiben (`open-task`) auf den Seiten, wo ein eigener Satz entsteht. Kein Ziehen von Karten (keine Komponente, `prefer-built-in-block`): `ordering` ersetzt es; ein Karten-Ziehen wäre ein Wunsch für ein Inkrement.
**Audio:** Skill `lernapps-audio`, Stimme `bf_emma` (britisch), ganze Sätze, das Ausklingen mit `regen_audio.py` (aus hello-millbrook) abschneiden, Namen am Satzende zweisilbig (Sophie, Peter, Ellie, Amir); keine Sätze zwischen Seiten wiederholen; Diktat 3 + Nachsprechen 3 je Seite (Wiederholungsseiten: kein Audio) = 54 Sätze; Liste `audio-texte.json`.
**Datendateien:** keine (jede Tatsache steht einmal in ihrer Seite). **Komponenten:** keine. **Selbsteinschätzung:** je Kapitel (`selfAssessment` in `chapter.yaml`, zwei Übungen je Seite).
**Ein späterer Agent** ergänzt Kapitel 4 (`emphase-do`, `inversion`, Stufe 9-10, keine erfundenen Kinder mehr, Beispiele aus Reden und Literatur) als Inkrement `increment/<NN>-<name>` nach dem Inhaltsführer (Abschnitt „Adding a chapter or round“).

## Code

<!--
- Build the app, locally on `work`, on your own. After each task: `plan done`, then one commit with the work and this
  plan. The hooks check each commit; a failing check is fixed from its message, as skill `lernapps-cli` says.
- What you cannot decide: choose, write it under "Key decisions" with "(guess)", go on.
- The creator asks for a change: say your reading in one sentence first, then change every place it holds for
  (`feedback-applied-everywhere`).
-->

### Tasks

- [ ] Load skill `lernapps-cli`. Create the app as its section "Create" says:
      `npx --no -- lernapps create --archetype explainer`.
- [ ] Fill the content guide `.agents/skills/app-content/SKILL.md` from "Notes" and "Content method": every heading,
      no "FILL IN" left. Commit it before any content.
- [ ] Load skill `lernapps-explainer`.
- [ ] Load skill `lernapps-content-questions`. Read whole, with your file tool:
      `.agents/skills/lernapps-explainer/references/blocks.md` and
      `.agents/skills/lernapps-explainer/references/exercises.md`. A foreign language: also
      `references/language-tasks.md` in the same folder. A component in the plan: also `references/components.md`.
- [ ] Decide whether the app needs `scope`, as "`scope`" in
      `.agents/skills/lernapps-explainer/references/structure.md` says. Write the choice under "Key decisions".
- [ ] Musterseite (simple-present-fragen) komplett bauen: App- und Kapitelgerüst (, ), Satzleiste-SVGs (, ), Szene, Abschnitte einstieg bis weiter, mindestens sechs Übungen, Audio (3 Diktat, 3 Nachsprechen); zeigt, wie eine Seite mit dem Helfer do aussieht.
<!-- tasks: pattern (1 added): the one page or screen that is the pattern for the others -->
- [ ] **Checkpoint:** the pattern page. Load skill `lernapps-learner-check` and do its learner check on the page. Fix
      what it finds. Then show the creator the page and ask whether the others may follow it. Stop and wait. A
      change: change the pattern first.
- [ ] Kapitel 1 : , (recap classroom-phrases), und mit Satzleiste-SVGs (, ), Szenen, Übungen und Audio.
- [ ] Kapitel 2 : (recap simple-present und to-be), , , , mit Satzleiste-SVGs, Szenen, Übungen und Audio; mit Selbsteinschätzung.
- [ ] Kapitel 3 : (recap simple-past), und mit Satzleiste-SVGs (, , ), Szenen, Übungen, Rückblick und Audio; mit Selbsteinschätzung.
- [ ] Start- und Kapitelseiten: (scope, intro, chapters), Selbsteinschätzung der App, Poster und Schulkalender wachsen über die Seiten; Audio-Liste vollständig.
<!-- tasks: pages (4 added): the other pages or screens, after the pattern -->
- [ ] Update the content guide so that it describes the app as built (`app-content-matches`).
- [ ] Run `npx --no -- lernapps check` until it passes.
- [ ] Look at every screen and state, at 360 px and on a desktop, as "Look at the app" of skill `lernapps-cli` says.
      Compare each with its sketch.
- [ ] Do the whole-app check of skill `lernapps-learner-check`. Fix what it finds and write under "Notes" what you
      fixed.

## Commit

<!--
- Put the app on GitHub, publish it with the creator's yes, then list it. A push to `main` publishes.
- Open the pull requests (to `main`, to the catalog) without asking: they publish nothing.
- The creator asked to stop before publishing (a trial): stop here and say so.
-->

### Tasks

- [ ] Load skill `lernapps-explainer-self-assessment`. Add the self-assessment as it says, or write under "Key
      decisions" why the app has none. Commit.
- [ ] Load skill `lernapps-github`. Set up the repository and Pages as it says. Ask for the repository's name and
      every click only the creator can make, in one message.
- [ ] Push `work`, open the preview pull request and see its checks to green, as skill `lernapps-github` says.
- [ ] **Checkpoint:** publish. Show what the app does and the preview link from the comment "Vorschau der App". Ask
      whether it may go online. Stop and wait for the yes.
- [ ] Load skill `lernapps-commit`. Publish as skill `lernapps-github` says: `work` into `main` as one squash commit,
      the run of `Pages` watched to its end.
- [ ] Open the address the job `deploy` printed and confirm that the app shows. Never use a derived address.
- [ ] Load skill `lernapps-listing`. Write the entry under "Entry draft" as it says, with the creator's answer to
      "Finding the app".
- [ ] Fill the retrospective.
- [ ] Commit this plan on `main` and push it: the listing check and the review read it there.
- [ ] **Checkpoint:** list. Open the listing pull request as skill `lernapps-listing` says, without asking first: the
      pull request is the review. See it to "bestanden", then show the creator the pull request and its result.
- [ ] If the plan changed since its last push, commit it on `main` and push again.

### Entry draft

<!-- YAML valid against the entry schema the listing skill names. Only known values, never invented. -->

```yaml
```

## Retrospective

<!-- At the end of Commit, before the listing pull request. Facts, short, no names. Read by review and evals. -->

### Phases reached

<!-- Last phase completed, checkpoints passed. E.g. "commit; confirmed, published". -->

### Creator turns after the plan

<!-- Number of creator messages after the confirmation, topic of each. Target: at most 3. -->

### Where I had to guess

<!-- Each gap in plan, skills, messages or answers, and your choice. "None" if none. -->
