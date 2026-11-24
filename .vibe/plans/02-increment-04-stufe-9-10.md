---
# Read by the hooks, the review, the evals. Schema: @lernapps/tooling/guidance/plan-front-matter.v1.schema.json
# Written by `lernapps plan` and the hooks. Never change a key or a value by hand.
# Archetype, as in the app's first plan. Allowed values: explainer, interactive, quiz.
archetype: explainer
# Current phase. Allowed values: explore, plan, code, commit.
phase: explore
# prePushFailures: failed pre-push runs of this increment, written by the hook.
prePushFailures: 0
# failedChecks: failed rules and runs, written by lernapps check and the hooks.
failedChecks: {}
---

# Increment: increment-04-stufe-9-10

<!--
For you, the assistant. One increment of a published app: new competencies, chapters, pages, rounds, questions, or a
correction. The process is in AGENTS.md; this plan holds the method.
- `npx --no -- lernapps plan next` prints the task to do now, `plan done` ticks it and prints the next one.
- You write only below Goal, Key decisions, Notes, Answers, Content method and Retrospective, in the creator's
  language. Delete the comment of a section once the section is filled.
- The first version's decisions stand: archetype, content method, content guide. Never change an earlier plan.
- Work on the branch `increment/<NN>-<short name>`. Until Commit everything is local: push nothing.
-->

*Started 2026-11-24. Explore, Plan, Code, Commit.*

## Goal

Die Lernenden (Klasse 9-10) betonen eine Aussage mit do, does oder did und verstehen und bilden Sätze, in denen Helfer und Subjekt nach einem verneinenden Wort (never, hardly, not only) die Plätze tauschen. Beides üben sie an zwei Sachtexten mit Daten und Quellen.

## Key decisions

- Kapitel 4 „Betonen und umstellen“ mit zwei Seiten: `emphase-do` (Betonung mit do) und `inversion`, je eine Seite je Baustein der Karte (Stufe 9-10, Schritt 1). Keine Wiederholungsseite: Alle `requires` (`simple-past-fragen`, `wortstellung`, `simple-present-fragen`) werden in Kapitel 1 bis 3 der App geübt.
- Form der Stufe 9-10 nach `konventionen.md`: je Seite ein Lesestück (300 bis 600 Wörter) als Kern, eigener Text nach Fakten, Randglossar als Vokabelblock, Aufgaben in drei Stufen (Verstehen, Belegen mit Zeile, Meinung/Schreiben), keine erfundenen Kinder, sachlicher Ton, Anrede „du“ (guess: Absprache für 9-10 steht aus; die Orchestrator-Session hat „du“ nicht widersprochen).
- Fälle (guess, Wahl nach Quellenlage): `emphase-do` am Fall Marie Curie (Zweifel und Belege, Nobelpreise 1903 und 1911), `inversion` an der Mondlandung von Apollo 11 (Daten zur Landung). Beide Fälle real, neutral, belegbar aus Wikipedia (nur Fakten); die Beispiele „aus Reden und Literatur“ des Issues ersetzt der eigene Text, weil keine Sätze aus fremden Texten übernommen werden dürfen.
- Figuren: Sophie, Ellie, Peter, Amir kommen nicht mehr vor; die Seiten sprechen „du“ an und führen keine Kinder ein.
- Bild: ein neues Bild je Seite nur, wo es etwas zeigt (Satzleiste mit dem Helfer: Betonung und Umstellung); die Satzleisten-Familie wächst um `satzleiste-emphase` und `satzleiste-inversion`.

## Notes

Neu, Strang `englisch/grammatik`, Band 9-10, Schritt 1, beide Lücken der Karte (`practisedBy` leer): `emphase-do` „Ich kann eine Aussage mit do, does oder did verstärken (I do like it!).“ (requires `simple-past-fragen`) und `inversion` „Ich kann nach Wörtern wie never, hardly und not only die Wortstellung umkehren, um etwas zu betonen.“ (requires `wortstellung`, `simple-present-fragen`). Alle Voraussetzungen übt die App schon (Kapitel 1 bis 3), darum kein `recap`. Kapitel `betonen-und-umstellen` („Betonen und umstellen“).
**Didaktik:** Die Satzleiste bleibt das eine wachsende Bild: Der Helfer, den die Lernenden als Frage- und Verneinungskarte kennen, steht auch in der Aussage, um etwas zu verstärken (eine gelbe Karte vor dem Verb, betont), und er springt nach einem verneinenden Wort nach vorn wie in einer Frage. Je Seite: Einstieg mit Vorwissen-Frage, Lesestück mit Randglossar, dann Verstehen, Belegen, Anwenden. `emphase-do`: Lesestück „Zweifel an Marie Curie“ (Zeitungsstil, ~320 Wörter, eigener Text nach Fakten: erste Frau mit Nobelpreis, zwei Nobelpreise in zwei Wissenschaften, 1903 und 1911, Professorin in Paris 1906); Betonung widerspricht einem Zweifel oder einer Annahme (She did win two Nobel Prizes, I do think …, He does exist.), nicht im Satz mit be und Modalverben. `inversion`: Lesestück „Landung auf dem Mond“ (Sachtext mit Daten, ~380 Wörter: Start 16. Juli 1969, Landung 20. Juli, 2 Std. 31 Min. 40 Sek. Mondspaziergang, mehr als 21 Stunden auf der Oberfläche, 21,5 kg Mondgestein, Rückkehr 24. Juli, rund 600 Millionen Zuschauer, 25 Sekunden Treibstoff); Muster: Never before have …, Hardly had … when …, Not only did … but … (nach dem Wort kommt die Frageform), mit Hinweis, dass die Umkehr gehobenes Englisch ist und in Reden und Texten vorkommt. Fehler, die die Rückmeldung fängt: emphatisches do + 3. Form (She does wins), did + 2. Form (did won), do ohne Betonung als Hilfsverb in der Aussage ohne Sinn, Inversion ohne Helfer (Never I have seen), Inversion mit Helfer UND Verb im Hauptsatz doppelt (Never did he went), Subjekt-Verb-Reihenfolge nach not only (Not only she won).
**Umfang:** drin: beide Bausteine, je ein Lesestück, Übungen, Diktat und Nachsprechen aus Sätzen des Lesestücks, Schreibauftrag; nicht drin: Inversion in Bedingungssätzen (Had I known …), Inversion nach so/such und nach Orts-Adverbien (Here comes …), emphatisches do im Imperativ (Do be quiet), Betonung durch Satzmelodie (#482). Alter: 9-10, Sprache Deutsch mit englischem Text.
**Quellen (am 2026-11-24 geöffnet, nur Fakten, keine Sätze):** Wikipedia (en) „Apollo 11“ (Daten, 600 Millionen Zuschauer, EVA-Dauer, Treibstoff, Mondgestein, Rückkehr), „Marie Curie“ (Nobelpreise, erste Frau mit Nobelpreis, Professorin in Paris 1906), „Do-support“ (emphatisches do), „Subject–auxiliary inversion“ (Inversion). Lernlandkarte Englisch (Bausteine). Grundwortschatz (A1/A2; Wörter darüber werden im Randglossar erklärt). Nicht geprüft: VOA, Wikinews (nicht gebraucht, eigene Texte).
**Neues Muster:** Das Lesestück (Konventionen Abschnitt 8) ist neu in dieser App; Aufbau und Blöcke kommen in den Inhaltsführer, wenn die Musterseite steht.

## Explore

<!--
- All content questions belong here; Plan maps the answers onto the app. Ask; write no code.
- Skip what earlier answers or the app already tell. At most 2 questions per message, one topic each.
-->

### Tasks

- [x] Read the README of the archetype's template (its path is in skill `lernapps-app`): what the app can do now.
      Tell the creator what is new, if it matters for this increment.
- [x] Load the content guide `.agents/skills/app-content/SKILL.md` and read the earlier plans in `.vibe/plans/`: what
      the app teaches, how its content is made, what is open.
- [x] Interview, one topic per question, the creator's words under "Answers": which competencies, chapters or rounds,
      for which school years; hurdles and examples; the amount; any change of look and feel or of terms. No answer:
      ask once more, then write your assumption with "(guess)".
- [x] Load skill `lernapps-content-research`. Research what the content guide does not cover. Write under "Notes":
      the new competencies by chapter with their ids, the sources you opened.
- [x] Write under "Notes" the didactic approach per competency and the scope (in, out, data range).
- [x] The increment needs a kind of content the guide does not cover (a new page structure, screen, component or kind
      of exercise): load skills `lernapps-explainer-design` and `lernapps-exercise-patterns`. Else skip this task.
- [ ] **Checkpoint:** research. Show in plain words: the new competencies by chapter, the didactic approach, the
      scope, every "(guess)", the sources and what is unchecked. Stop and wait. Changes: change them, then ask again.

### Answers

- Auftrag (Orchestrator-Session in der Rolle der Ersteller:in, mit Zustimmung der Ersteller:in zum Push von 417e2bc): Kapitel 4 „Betonen und umstellen“ (Stufe 9-10) als Inkrement `increment/04-stufe-9-10` bauen, wie bei den Inkrementen 7-8: Plan-Checkpoint, Musterseite, Gesamtcheck und Sprachprüfung mit Sub-Agenten, Vorschau-PR, nicht mergen; Regeln der `konventionen.md` (keine Figuren-Einführung im Seitentext, Vokabelblock, Hörurteile bestätigt der Orchestrator); Tooling vorher auf den neuesten Stand.
- Inhalt und Umfang: laut Issue #473 Kapitel 4, Bausteine `emphase-do` und `inversion`.

## Plan

<!--
- Map the new content onto the app with the guide's patterns. The creator confirms the plan in one read.
- After the yes you work on your own.
-->

### Tasks

- [ ] Load skill `lernapps-content-growth`. Add the tasks of Code as slices, one per competency, in the guide's
      order, one call each: `npx --no -- lernapps plan add --at slices "<task>"`. Say in each which sub-agent may
      write it in parallel, if any.
- [ ] Write "Content method": the guide's patterns, figures and components per slice. Anything new: map it as skill
      `lernapps-explainer-design` says, and say why the guide's patterns do not fit.
- [ ] Draw a sketch of each new component or interactive exercise, in `.vibe/sketches/`.
- [ ] Show the creator, short: goal, new competencies by chapter, slices; in plain words what learners see and do and
      what is new. At most 2 questions.
- [ ] **Checkpoint:** confirm the plan and the content method. Stop and wait for an explicit yes. Changes: change
      them, then ask again.

### Content method

<!-- One line each: the guide's patterns, figures and components used, and where; anything new, what it does and
cannot. Something new goes into the guide in the slice that adds it. -->
<!-- An explainer: per figure, model and component its learning action in two to four sentences
(`explainer-representation-explained`); per page its prerequisites the app does not practise, and which get a recap
page, which a link. -->

## Code

<!--
- Build locally on the branch, on your own. After each task: `plan done`, then one commit with the work and this
  plan. The hooks check each commit; a failing check is fixed from its message, as skill `lernapps-cli` says.
- What you cannot decide: choose, write it under "Key decisions" with "(guess)", go on.
- The creator asks for a change: say your reading in one sentence first.
-->

### Tasks

- [ ] `git switch -c increment/<NN>-<short name>` from `main`. Commit this plan on it.
- [ ] Load skill `lernapps-cli`. Update the app as its section "Update" says. Commit the update alone and fix its
      findings before any content. The update replaces the `lernapps-*` skills: read again those you use.
- [ ] Load skill `lernapps-explainer` and the content guide.
- [ ] Load skill `lernapps-content-questions`. Read whole, with your file tool:
      `.agents/skills/lernapps-explainer/references/blocks.md` and
      `.agents/skills/lernapps-explainer/references/exercises.md`. A foreign language: also
      `references/language-tasks.md` in the same folder. A component in the plan: also `references/components.md`.
- [ ] Decide whether the app needs `scope`, as "`scope`" in
      `.agents/skills/lernapps-explainer/references/structure.md` says. Write the choice under "Key decisions".
<!-- tasks: slices: one per competency, as written in Plan -->
- [ ] **Checkpoint:** the pattern page, after the first slice. A slice in a pattern the app already has: show it to
      the creator and go on. A new pattern: load skill `lernapps-learner-check`, do its learner check, fix what it
      finds, then ask the creator whether the others may follow it, and wait.
- [ ] Update the content guide so that it describes the app as it is now (`app-content-matches`).
- [ ] Run `npx --no -- lernapps check` until it passes.
- [ ] Look at every changed screen, at 360 px and on a desktop, as "Look at the app" of skill `lernapps-cli` says.

## Commit

<!--
- Publish with the creator's yes. A push to `main` publishes.
- Open the pull requests (to `main`, to the catalog) without asking: they publish nothing.
-->

### Tasks

- [ ] If pages or exercises changed, load skill `lernapps-explainer-self-assessment` and update the self-assessment
      as it says. Commit.
- [ ] Load skill `lernapps-github`. Push the branch, open the preview pull request and see its checks to green, as it
      says.
- [ ] **Checkpoint:** publish. Show what the increment adds and the preview link. Ask whether it may go online. Stop
      and wait for the yes.
- [ ] Load skill `lernapps-commit`. Publish as skill `lernapps-github` says: the pull request squash-merged into
      `main`, the run of `Pages` watched to its end.
- [ ] Open the address the job `deploy` printed and confirm the new content. Never use a derived address.
- [ ] The app is listed and its entry changes (school years, summary): load skill `lernapps-listing` and write the
      changed entry. Else skip this task.
- [ ] Fill the retrospective.
- [ ] Commit this plan on `main` and push it. A push of only `.vibe/` publishes nothing.
- [ ] **Checkpoint:** list. The entry changed: open the pull request to the catalog as skill `lernapps-listing`
      says, without asking first, see it to "bestanden", then show the creator the pull request and its result. The
      entry did not change: tell the creator that the catalog updates the app by itself.
- [ ] If the plan changed since its last push, commit it on `main` and push again.

## Retrospective

<!-- At the end of Commit. Facts, short, no names. Read by review and evals. -->

### Phases reached

<!-- Last phase completed, checkpoints passed. E.g. "commit; confirmed, published". -->

### Creator turns after the plan

<!-- Number of creator messages after the confirmation, topic of each. Target: at most 3. -->

### Where I had to guess

<!-- Each gap in plan, skills, content guide, messages or answers, and your choice. "None" if none. -->
