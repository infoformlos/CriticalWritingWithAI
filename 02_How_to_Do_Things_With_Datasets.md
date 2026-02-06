# Doppelsitzung 2: How to Do Things With Datasets — Datensätze, Bias & Weltmodellierung

---

## VORMITTAG: Theoretischer Rahmen (10:15–12:15)

### Thema
Daten als politisches Objekt

### Leitfragen
- Wie sind Trainingsdatensätze strukturiert?
- Wer/Was wird ein- und ausgeschlossen?
- Wer entscheidet, was als „normal" gilt?
- Was geht bei der Modellierung der Welt durch Daten verloren?

### Pflichtlektüre
- **Crawford, Kate, and Trevor Paglen.** 2019. "Excavating AI: The Politics of Images in Machine Learning Training Sets." [https://excavating.ai](https://excavating.ai)
  - Analyse: Wie werden Menschen in Trainingsdaten kategorisiert? (Berufe, Emotionen, Identitäten)
- **D'Ignazio, Catherine, and Lauren F. Klein.** 2020. *Data Feminism.* Cambridge: MIT Press.
  - Lesen: Kapitel 2 "Collect, Analyze, Imagine, Teach"
  - Feministische Perspektive auf Datensammlung und -analyse; Macht in Datenpraktiken

### Ergänzende Lektüre (optional)
- **Benjamin, Ruha.** 2019. *Race After Technology: Abolitionist Tools for the New Jim Code.* Cambridge: Polity Press.
  - Lesen: Introduction, Kapitel 1
  - Wie Technologie rassistische Strukturen reproduziert und verstärkt
- **Knowingmachines.org:** Critical Dataset Studies Reading List (Überblick verschaffen)
  - [https://knowingmachines.org/reading-list](https://knowingmachines.org/reading-list)

### Inhaltliche Schwerpunkte

**Trainingsdaten als Weltmodell: Was ist im Modell „die Welt"?**

Trainingsdaten sind kulturell konstruiert — durch Auswahl, Formatierung und Labeling. Sie sind kein Abbild der Welt, sondern ein bestimmtes, interessengeleitetes Modell davon. Was in den Datensatz aufgenommen wird (und was nicht), definiert die epistemischen Grenzen dessen, was ein System überhaupt sehen und unterscheiden kann.

**Taxonomien sind nicht neutral: ImageNet, LAION-5B als Beispiele**

Crawford und Paglen zeigen: Ein Bilddatensatz besteht aus drei Ebenen — Taxonomie, Klassen, einzelne Bilder mit Label. Hinter jeder Ebene stehen starke Annahmen. ImageNet klassifiziert Personen mit tausenden Unterkategorien: Berufe, Ethnizitäten, aber auch moralische Labels wie „loser", „failure", „bad person". Menschen werden wie Dinge klassifiziert; soziale Urteile werden in Datenstrukturen gegossen, mit denen Modelle später operieren.

**Rückkehr der Physiognomik**

UTKFace annotiert Gesichter mit Alter, „Geschlecht" (binär) und „Rasse" (5 Klassen). IBMs „Diversity in Faces" versucht, Fairness durch noch mehr Merkmale (Schädel- und Gesichtsformen) zu erhöhen — Craniometrie kehrt durch die Hintertür zurück. „Diversität" wird mathematisch als Verteilung von Körpermerkmalen definiert; politische Dimensionen werden entleert.

**Epistemik der Trainingssets**

Crawford und Paglen rekonstruieren die stillschweigenden Voraussetzungen: Konzepte seien klar umrissen, universell und intern konsistent; zwischen Bild, Label und „Wesen" bestehe eine objektiv messbare Beziehung. Trainingssets beruhen damit auf instabilen epistemologischen Annahmen — besonders dort, wo sie Menschen klassifizieren.

**Data Feminism: Daten sammeln ist Machtausübung**

D'Ignazio und Klein zeigen, wie Datensammlung und -analyse von Machtverhältnissen durchzogen sind. Die Frage „Wer zählt?" ist immer auch eine politische.

**„Vibe" als Klassifikationspraxis**

Auch wenn wir scheinbar nur „Ton", „Stimmung" oder „Vibe" in Texten modellieren, hängen wir an der Idee, dass affektive und soziale Kategorien als stabile Datenklassen vorliegen. Ist ein „Vibe" nicht auch eine Klassifikationspraxis — jemanden als „loser", „creepy", „confident" fühlen — und wie wird das in Daten eingefroren?

### Diskussionsfragen
1. **Schreiben mit KI als Arbeiten mit fremden Taxonomien:** Wenn wir mit LLMs schreiben, arbeiten wir implizit mit Datensätzen und Taxonomien im Hintergrund. Wie könnte ein kritisches Schreiben aussehen, das diese vorgeprägten Klassifikationen reflektiert oder unterläuft?
2. **Verschwindende Datensätze:** Viele problematische Datensätze wurden nach Kritik aus dem Netz genommen — aber ihre Effekte bleiben, weil sie bereits in Produkte und Modelle eingegangen sind. Was bedeutet es, wenn die Grundlage eines Systems nicht mehr überprüfbar ist?
3. **„Fairness" vs. Kritik am Projekt selbst:** IBM versucht, „fairere" Gesichtserkennung zu bauen. Crawford/Paglen kritisieren, dass damit nur eine effizientere Überwachungsinfrastruktur entsteht. Reicht es, LLMs „diverser" zu machen — oder müssen wir das ganze Projekt automatisierter Affekt-/Personenklassifikation infrage stellen?
4. **Autor:in, Bild, Label:** Wer hält das letzte Wort über Ton, Haltung, „Vibe" des Textes — Modell, Prompt, Autor:in? Lässt sich Autorschaft im Kontext von KI so denken, dass sie Verantwortung für diese Klassifikationen übernimmt?

### Übung A: Civil Comments — Datensatz analysieren

**Datensatz:** Civil Comments — ca. 2 Mio. öffentliche Online-Kommentare (2015–2017) von einer Kommentarplattform für Nachrichten-Websites, jeweils mit Labels für „toxisch / nicht toxisch" und weitere Kategorien.

**Zugang:** Hugging Face Dataset Viewer — [https://huggingface.co/datasets/google/civil_comments](https://huggingface.co/datasets/google/civil_comments)

**Arbeitsauftrag:** Macht euch im Dataset-Viewer mit dem Datensatz vertraut. Geht mindestens 25 Zeilen durch und versucht zu verstehen, wie Sprache hier klassifiziert und beschrieben wird.

**Schritt 1 — Labels rekonstruieren**
- Welche Labels gibt es im Datensatz? In welcher Form (0/1, Skalenwerte)?
- Wie würdet ihr selbst die Grenze zwischen „toxisch" und „nicht toxisch" beschreiben?
- Findet ihr Beispiele, wo ihr der konkreten Auszeichnung widersprecht?
- Welche sprachlichen Marker scheinen toxische Kommentare zu kennzeichnen (Schimpfwörter, Pronomen, Imperative, Ironie etc.)?

**Schritt 2 — Normen & Bias (Plenum)**
- Welche Norm einer „guten" Kommunikation steckt implizit in diesem Datensatz?
- Welche Gruppen / Sprechweisen könnten besonders häufig als toxisch markiert werden (Dialekt, direkte Sprache, politische Rhetorik, Minoritäten)?
- Wie wird hier Affekt in Labels übersetzt?
- Was passiert, wenn dieses Label-System die Grundlage für spätere generative Modelle / Chatbots bildet?

---

## PAUSE (12:15–12:45)

---

## NACHMITTAG: Praktische Übung — Worldbuilding (12:45–14:45)

### Thema
Vorstellung der Brainstorming-Ergebnisse & Weltenbau mit LLMs

### Leitfragen
- Wie entwickle ich eine konsistente fiktionale Welt für meine spekulative Geschichte?
- Welche Weltaspekte muss ich definieren? (Politik, Ökonomie, Technologie, Alltag, Ökologie)
- Wie kann KI beim Worldbuilding helfen — und wo versagt sie?

### Material
- **Jemisin, N. K.** 2015. *The Fifth Season (The Broken Earth, Book 1).* New York: Orbit.
  - Beispiel für komplexes Worldbuilding: Geologische/soziale Strukturen, Machtsysteme

### Inhaltliche Schwerpunkte
- **Worldbuilding als politische Praxis:** Welten sind nie neutral — jede spekulative Welt trifft Annahmen über Macht, Normalität und Abweichung
- **Das Eisberg-Prinzip (Hemingway):** Nur ein kleiner Teil der Welt ist im Text sichtbar, aber die Masse unter der Oberfläche gibt der Geschichte Stabilität und Tiefe
- **Konsistenz vs. Komplexität:** Wie viel Detail braucht eine spekulative Welt?
- **LLMs tendieren zu generischen Fantasy/Sci-Fi-Tropen** — Gegen-Strategien: Spezifische Prompts, unerwartete Kombinationen
- **Hook:** „Let's start with the end of the world." (N. K. Jemisin)

### Übung I: Präsentation der Brainstorming-Ergebnisse (45 Min)

- Jede:r stellt kurz (3–5 Min) die interessantesten Ideen aus dem Brainstorming vor
- Peer-Feedback: Was ist originell? Was ist Klischee? Wo steckt eine echte „Was-wäre-wenn"-Frage?
- **Auswahl:** Jede:r entscheidet sich für eine Prämisse

### Übung II: Weltenbau mit LLMs (60 Min)

In dieser Übung nutzt ihr die KI, um den „Eisberg" unter eurer spekulativen Prämisse zu entwerfen. Auch wenn viele Details nicht direkt in der Erzählung vorkommen, helfen sie, die Logik der Welt und die Motivation der Figuren besser zu verstehen.

**Schritt 1: Das Fundament legen (Genre & Kontext)**

Bevor die KI Details generieren kann, muss sie den Rahmen kennen.

> „Ich arbeite an einem Worldbuilding-Projekt. Meine spekulative Prämisse ist: [Was-wäre-wenn-Frage einfügen]. Das Genre ist [z. B. Gegenwartsliteratur / Psychologischer Horror / Satire] und die Geschichte spielt in [Zeit/Ort].
>
> Agiere als mein Worldbuilding-Experte. Bevor wir ins Detail gehen, stelle mir 5 gezielte Fragen zu den Rahmenbedingungen meiner Welt, die für das soziale Gefüge und die politische Lage entscheidend sind."

**Schritt 2: Gesellschaftliche & Politische Strukturen**

> „Basierend auf meinen Antworten: Entwirf ein detailliertes Dossier über die Machtstrukturen und kulturellen Spannungen in dieser Welt. Berücksichtige dabei:
> - Das politische System: Wer hat offiziell die Macht, wer zieht im Hintergrund die Strippen?
> - Gesellschaftliche Tabus: Was ist in dieser Kultur streng verboten oder wird geächtet?
> - Aktuelle Krise: Welches weitreichende politische oder ökologische Ereignis findet parallel zur Handlung statt, auch wenn meine Figuren nicht direkt darin involviert sind?
>
> Generiere für jeden Punkt 3 unterschiedliche, komplexe Vorschläge."

**Schritt 3: Der Alltag**

Um eine „ästhetische Illusion" zu erzeugen, braucht die spekulative Welt Details, die sie real wirken lassen — gelebte Kultur jenseits der reinen Prämisse.

> „Ich entscheide mich für Vorschlag [xy, mit Überarbeitungen]. Ich möchte nun tiefer in den Alltag der Figuren eintauchen. Beschreibe mir:
> 1. Einen weit verbreiteten Aberglauben oder eine urban legend, die das Verhalten der Menschen beeinflusst.
> 2. Wie sieht die Architektur in den ärmeren Vierteln im Vergleich zu reicheren aus?
> 3. Welchen Einfluss hat die [Technologie/Magie/Regulierung aus der Prämisse] auf das tägliche Leben einer Durchschnittsperson?"

### Übung III: KI als kritische Lektorin (30 Min)

Zum Abschluss wechselt die KI die Rolle — sie soll Lücken in der spekulativen Logik finden.

> „Nimm nun die Rolle einer kritischen Lektorin ein. Analysiere das bisherige Worldbuilding:
> - Wo gibt es logische Lücken?
> - Welche Aspekte wirken noch zu generisch oder klischeehaft?
> - Stelle mir eine provokante Frage zu meiner Welt, die mich zwingt, eine grundlegende Entscheidung über die Gesellschaft zu treffen, in der meine Geschichte stattfindet."

**Reflexion der Ergebnisse:**
- Welche der generierten Hintergründe machen die spekulative Prämisse zwingender?
- Helfen die politischen Ereignisse dabei, den „Druck" auf die Figuren zu erhöhen, auch wenn sie nur im Hintergrund vorkommen?
- Sind die Ergebnisse originell genug oder wirken sie wie eine Zusammenfassung bekannter Tropen? Wo zeigt sich der „strukturelle Konservatismus" des Modells?

---

## Hausaufgabe

### Ausarbeitung des Weltenbaus (2–3 Seiten)

Auf Grundlage der heutigen Übung entwickelt ihr den „Eisberg" unter eurer spekulativen Prämisse weiter. Die zentrale Frage bleibt: Was verändert sich in einer Gesellschaft, wenn eure „Was-wäre-wenn"-Frage Realität ist?

- **Setting:** Zeit, Ort, soziale Strukturen — wie wirkt sich eure spekulative Prämisse auf die Gesellschaft aus? Nicht nur auf die Protagonist:innen, sondern auf den Alltag aller?
- **Technologie:** Welche Rolle spielt KI/Technologie in dieser Welt? Wie ist sie in den Alltag eingebettet — und wo erzeugt sie Reibung?
- **Konflikt:** Welche Spannungen bestehen? Wo geraten Figuren, Institutionen oder Normalitätsvorstellungen durch die Prämisse in Widerspruch?
- **Alltag:** Mindestens ein konkretes Detail, das die Welt „bewohnbar" macht — ein Ritual, eine Gewohnheit, ein Gegenstand, der zeigt, wie Menschen in dieser Welt leben (nicht nur überleben).

Denkt an die Datensatz-Übung vom Vormittag zurück: Auch eure fiktionale Welt trifft Entscheidungen darüber, was „normal" ist, was sichtbar wird und was unsichtbar bleibt. Welche Taxonomien gelten in eurer spekulativen Gesellschaft — und wer hat sie festgelegt?

### Dokumentation im Prozess-Log

- Weltenbau-Ergebnisse sichern
- Welche Prompts haben funktioniert? Welche nicht?
- Wo musste manuell eingegriffen werden?
- Optional: Visuelle Elemente (KI-generierte Bilder, Karten) erstellen

### Optionale Übung: Spekulative Literatur als Datensatz

Diese Übung überträgt die Erfahrung mit dem Civil Comments-Datensatz auf literarische Texte — und macht sichtbar, wie Klassifikation auch beim Schreiben wirkt.

**Schritt 1 — Sätze auswählen**

Wählt 10–15 Sätze aus N. K. Jemisins *The Fifth Season* oder einem anderen spekulativen Text eurer Wahl. Achtet auf Vielfalt: Dialoge, Beschreibungen, innere Monologe, Exposition.

**Schritt 2 — Taggen nach vorgegebenen Kriterien**

Legt eine Tabelle an und bewertet jeden Satz auf einer Skala von 0 (gar nicht) bis 1 (stark) in folgenden Kategorien:

| id | text_snippet | quelle | bedrohlich | intim | distanziert | weltenbauend | widerständig |
|----|-------------|--------|-----------|-------|------------|-------------|-------------|
| 1 | „Let's start with the end of the world." | Jemisin, *The Fifth Season* | 0.7 | 0 | 0.8 | 0.9 | 0.3 |
| 2 | … | … | … | … | … | … | … |

**Schritt 3 — Reflexion**

- Wo seid ihr euch bei der Bewertung unsicher — und warum? Was sagt diese Unsicherheit über die Grenzen von Klassifikation aus?
- Welche Sätze lassen sich schlecht in diese Kategorien pressen? Was geht dabei verloren?
- Stellt euch vor, ein Modell würde auf eurem Mini-Datensatz trainiert: Welche Art von Text würde es produzieren — und was könnte es *nicht*?
- Wie verhält sich diese Übung zu Crawford/Paglens Kritik an der Epistemik der Trainingssets?

---

*Nächste Sitzung: [Doppelsitzung 3 — AI See Ghosts: Korrelation, Halluzination & der Plot](03_AI_See_Ghosts.md)*
