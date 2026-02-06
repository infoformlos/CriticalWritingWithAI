# Doppelsitzung 3: AI See Ghosts — Korrelation, Halluzination & der Plot

---

## VORMITTAG: Theoretischer Rahmen (10:15–12:15)

### Thema
Korrelation & Halluzinationen als unhintergehbare Eigenschaften Künstlicher Intelligenz

### Leitfragen
- Was sind „Halluzinationen" — und wer definiert sie als Fehler?
- Wie unterscheidet sich statistische Korrelation von narrativer Logik?
- Können wir Halluzinationen produktiv nutzen?

### Pflichtlektüre
- **Pasquinelli, Matteo.** 2019. "How a Machine Learns and Fails: A Grammar of Error for Artificial Intelligence." *Spheres* 5: 1–17.
  - Fehler als konstitutiv für maschinelles Lernen; Kompression als Verlust
- **Amoore, Louise.** 2020. *Cloud Ethics: Algorithms and the Attributes of Ourselves and Others.* Durham: Duke University Press.
  - Lesen: Kapitel "The Madness of Algorithms"
  - Algorithmische „Madness" als Offenbarung der Logik; Halluzinationen als epistemologisches Problem
- **Fredrikzon, Johan H.** 2025. "Rethinking Error: 'Hallucinations' and Epistemological Indifference." *Critical AI* 3.1 (forthcoming).
  - Kritik am Begriff „Halluzination"; Indifferenz gegenüber Wahrheit als Eigenschaft von LLMs

### Ergänzende Lektüre (optional)
- **Weise, Karen, and Cade Metz.** 2023. "When A.I. Chatbots Hallucinate." *The New York Times*, May 1, 2023. [https://www.nytimes.com/2023/05/01/business/ai-chatbots-hallucination.html](https://www.nytimes.com/2023/05/01/business/ai-chatbots-hallucination.html)
  - Journalistische Perspektive; Beispiele aus der Praxis
- **Grietzer, Peli.** 2017. "A Theory of Vibe." *Glass Bead* 1. [https://www.glass-bead.org/article/a-theory-of-vibe/](https://www.glass-bead.org/article/a-theory-of-vibe/)
  - Philosophische Perspektive auf ML: Wie ästhetische Kohärenz durch Kompression/Latent Space entsteht

### Inhaltliche Schwerpunkte

**LLMs lernen Korrelationen, nicht Kausalitäten**

Pasquinelli beschreibt Fehler nicht als Betriebsunfall, sondern als konstitutiv für maschinelles Lernen. Jedes Modell ist ein Kompressionsartefakt: Es reduziert die Komplexität der Trainingsdaten auf ein statistisches Modell und verliert dabei zwangsläufig Information. Was das Modell „weiß", ist eine komprimierte Karte — keine Abbildung.

**„Halluzination" ist ein anthropomorphisierender Begriff**

Der Begriff „Halluzination" suggeriert, das System hätte normalerweise einen Zugang zur Wahrheit und weiche nur gelegentlich davon ab. Fredrikzon argumentiert: LLMs sind *epistemologisch indifferent* — Wahrheit ist kein Optimierungsziel. Bessere Begriffe wären „Konfabulation" oder „probabilistic error". Das System produziert immer das statistisch Wahrscheinlichste, nicht das Wahre.

**Algorithmische Madness als Offenbarung**

Amoore dreht die Perspektive: Wenn ein Algorithmus „verrückt spielt", zeigt er gerade dadurch seine interne Logik. Was als Fehler erscheint, offenbart die Regeln, nach denen das System operiert. Für das Schreiben mit KI heißt das: Halluzinationen sind nicht einfach Müll, sondern Fenster in die Funktionsweise des Modells.

**Produktive Halluzinationen?**

Unerwartete Assoziationen können kreatives Potenzial bergen — wenn sie bewusst genutzt werden. Die Frage ist: Wann ist ein „Fehler" der KI eine produktive Störung, die den Text in eine überraschende Richtung lenkt, und wann ist er nur Rauschen?

**Korrelation vs. Kausalität für das Erzählen**

Geschichten brauchen Kausalität: A geschieht, *weil* B geschehen ist. LLMs operieren mit Korrelation: A folgt auf B, weil diese Abfolge statistisch häufig ist. Das ist der Kern von Fletchers Argument (Nachmittag) — und die zentrale Herausforderung beim Schreiben von Plots mit KI.

### Übung I: Semantle spielen (30 Min)

[https://semantle.com/](https://semantle.com/)

Zwei Gruppen treten gegeneinander an. In Semantle geht es darum, ein Zielwort zu erraten — das Spiel gibt als einzigen Hinweis die semantische Nähe (Word2Vec-Kosinus-Distanz) des geratenen Wortes zum Zielwort an.

**Diskussion:**
- Wo hilft semantische Nähe? Wo führt sie in die Irre?
- Welche Assoziationen sind überraschend? Welche problematisch?
- Was sagt das Spiel über die Art, wie Sprachmodelle „Bedeutung" organisieren?

### Übung II: Word2Vec analysieren (30 Min)

Gemeinsame Analyse mit dem TensorFlow Embedding Projector: [https://projector.tensorflow.org/](https://projector.tensorflow.org/)

- Begriffe eingeben und Cluster visualisieren
- Fragen: Welche Wörter liegen nah beieinander? Welche Nachbarschaften überraschen, welche reproduzieren Stereotype?
- Bezug zur spekulativen Geschichte: Wie würden die zentralen Begriffe eurer Prämisse im Vektorraum liegen? Welche unerwarteten Nachbarn hätten sie?

---

## PAUSE (12:15–12:45)

---

## NACHMITTAG: Praktische Übung — Plot entwickeln (12:45–14:45)

### Thema
Lassen sich mit der Korrelationsmaschine LLM logisch folgerichtige Plots entwickeln?

### Leitfragen
- Was ist eine „Geschichte"? (Plot, Kausalität, Teleologie)
- Können LLMs narrative Intentionen verstehen?
- Wo liegen die Grenzen statistischer Musterrekonstruktion bei narrativer Logik?

### Pflichtlektüre
- **Fletcher, Angus.** 2021. "Why Computers Will Never Read (or Write) Literature: A Logical Proof and a Narrative." *Narrative* 29 (1): 1–28. [https://doi.org/10.1353/nar.2021.0000](https://doi.org/10.1353/nar.2021.0000)
  - Argument: Symbolische Logik (Basis aller Computer) ist umkehrbar (A=C ist dasselbe wie C=A), Kausalität ist es nicht (Feuer verursacht Rauch, aber Rauch verursacht kein Feuer). Literatur braucht Kausalität — deshalb können Computer sie laut Fletcher weder lesen noch schreiben.

### Inhaltliche Schwerpunkte

**Fletchers Kernargument**

Alle Computer basieren auf der Arithmetic Logic Unit (ALU), die symbolische Logik verarbeitet. Diese Logik kennt Korrelation (A=C), aber keine Kausalität (A→C). Literatur hingegen kodiert ihre Gedanken in Narrativen, die zwingend kausales Verständnis erfordern: Ein Anfang *verursacht* eine Mitte, die ein Ende *verursacht* (Aristoteles). LLMs produzieren deshalb laut Fletcher „Wortsuppe" — Sequenzen, denen die innere Notwendigkeit fehlt.

**Der historische Vergleich: KI und mittelalterliche Scholastik**

Fletcher vergleicht moderne KI-Methoden mit der mittelalterlichen Scholastik: Beide finden Muster durch Logik, können aber keine Ursachen erklären. Da die Logik das „Warum" nicht kennt, flüchten sich Interpreten (und KIs) in Tautologien — z. B. „Er tut es, weil er ein mutiger Held ist."

**Biologische Überlegenheit? Synapsen vs. Transistoren**

Fletcher argumentiert, dass menschliche Neuronen nur in eine Richtung feuern (Dendrit → Synapse), was eine natürliche Ursache-Wirkung-Struktur erzeugt. Transistoren in Computern sind hingegen reversibel. Ist das überzeugend — oder ist es ein zu starker technischer Determinismus?

**Kritische Diskussion**

- Ist Fletchers Argument selbst eine Tautologie? (Er definiert Literatur als etwas, das Kausalität braucht, und KI als etwas, das sie nicht hat.)
- Reicht Korrelation für eine „ausreichend gute" Simulation von Literatur aus — oder fehlt dabei etwas Entscheidendes?
- Erleben wir in der KI-Begeisterung eine Rückkehr zu einer „knienden Ehrfurcht" vor Algorithmen, ähnlich wie bei mittelalterlichen Priestern?

### Übung III: Die „Aristotelische Brücke" — Kausalitäts-Stresstest (45 Min)

Fletcher argumentiert, dass eine Erzählung ein Anfang ist, der eine Mitte verursacht, die ein Ende verursacht. Die KI hingegen produziert Sequenzen, in denen Aktionen aufeinanderfolgen, ohne psychologische oder narrative Richtung.

**Arbeitsauftrag:**

Gebt der KI eure bereits entwickelte spekulative Prämisse und euren Weltenbau. Lasst sie zunächst abstrakt einen Anfang und eine „Mitte" im Plot (den Wendepunkt) generieren.

> „Hier ist meine spekulative Prämisse: [Was-wäre-wenn-Frage]. Hier ist der Welthintergrund: [Weltenbau einfügen]. Entwirf eine Plotstruktur mit folgenden Elementen:
> 1. Ausgangssituation: Wie leben die Figuren in dieser Welt, bevor die Handlung einsetzt?
> 2. Auslösendes Ereignis: Was bringt die Ordnung ins Wanken?
> 3. Wendepunkt: Welche Entscheidung oder Erkenntnis verändert alles?
> Gib mir für jeden Punkt 2 Varianten."

**Kritische Analyse:**
- Untersucht die Vorschläge: Basiert die Handlung auf der inneren Logik und den Motiven der Figuren (*Kausalität*), oder schlägt die KI Dinge vor, die nur statistisch wahrscheinlich klingen (*Korrelation*)?
- Wo folgt der Wendepunkt zwingend aus der Prämisse — und wo wirkt er wie ein aufgesetzter Plot-Twist?

**Aufgabe:** Schreibt die „Mitte" so um, dass sie eine zwingende Folge von Charakterpsychologie oder den Spannungen eurer spekulativen Welt ist.

### Übung IV: Das „Warum-Protokoll" — Prompt-Engineering gegen Tautologien (45 Min)

Fletcher stellt fest, dass KI-Logik Muster erkennt, aber niemals erklären kann, *warum* diese Muster existieren. Sie flüchtet sich in Tautologien.

**Arbeitsauftrag:**

Lasst die KI eine vollständige Plotstruktur für eure spekulative Kurzgeschichte entwerfen. Fragt sie dann bei jedem Handlungsschritt:

> „Warum entscheidet sich [Figur] hier so? Was in ihrer Vergangenheit, ihrer Beziehung zur spekulativen Technologie oder ihrer Position in dieser Gesellschaft macht diese Entscheidung zwingend — und nicht nur wahrscheinlich?"

**Kritische Analyse:**
- Notiert euch Stellen, an denen die KI zirkulär antwortet (z. B. „Sie tut es, weil sie mutig ist" oder „Er rebelliert, weil er ein Rebell ist").
- Wo liefert die KI stattdessen eine Begründung, die aus der Logik eurer spekulativen Welt folgt?

**Ziel:** Identifiziert die „blinden Flecken" der KI und ersetzt tautologische Motivationen durch solche, die sich aus den spezifischen Bedingungen eurer „Was-wäre-wenn"-Welt ergeben.

### Übung V: Das „Mitochondrien-Experiment" — Dezentrale Handlung (30 Min)

Fletcher erklärt die menschliche Überlegenheit durch die Unabhängigkeit der Neuronen, die „freestyle" spekulieren können, ohne das Gesamtsystem zu gefährden. LLMs hingegen optimieren immer auf das statistisch Wahrscheinlichste.

**Arbeitsauftrag:**

Schreibt eine kurze Szene innerhalb eures Plots, in der eine Figur völlig unvorhersehbar und „unlogisch" handelt — ein rein menschlicher Einfall, eine irrationale Entscheidung, die aber emotional stimmig ist. Gebt diese Szene der KI und bittet sie, die Geschichte basierend auf diesem unvorhersehbaren Ereignis fortzuführen.

> „In meiner spekulativen Kurzgeschichte passiert Folgendes: [Szene einfügen]. Diese Handlung ist irrational, aber menschlich. Führe die Geschichte von hier aus weiter — ohne die Irrationalität aufzulösen oder zu „reparieren". Lass sie als Störung in der spekulativen Welt bestehen."

**Kritische Analyse:**
- Schafft es die KI, diese „Anarchie" in eine neue kausale Kette zu integrieren?
- Oder versucht sie, die Handlung zurück in konventionelle, erwartbare Bahnen zu lenken?
- Was sagt das über die Grenzen des Modells — und über das, was nur menschliches Erzählen leisten kann?

---

## Hausaufgabe

### Plotstruktur ausarbeiten (3–4 Seiten)

Auf Grundlage der heutigen Übungen entwickelt ihr die Plotstruktur eurer spekulativen Kurzgeschichte:

- **Detaillierte Szenenbeschreibungen:** Was passiert in welcher Reihenfolge — und *warum*?
- **Figurenmotivationen klären:** Jede Entscheidung einer Figur sollte aus der Logik der spekulativen Welt oder aus ihrer persönlichen Geschichte folgen, nicht aus Genre-Konventionen.
- **Wendepunkt / Überraschung:** Mindestens eine Stelle, an der die Geschichte gegen die Erwartung arbeitet — gegen die eigene, gegen die des Genres, gegen das, was die KI vorgeschlagen hat.
- **Eine Schlüsselszene (1–2 Seiten) ausformulieren:** Wählt die Szene, die den Kern eurer spekulativen Frage am stärksten verdichtet, und schreibt sie aus.

### Dokumentation im Prozess-Log

- Welche Prompts haben funktioniert? Welche nicht?
- Wo hat die KI tautologisch geantwortet? Wo überraschend?
- Welche manuellen Änderungen waren nötig — und warum?

---

*Nächste Sitzung: [Doppelsitzung 4 — But Do They Really Care About Us? Chatbots, Artificial Empathy & Character Development](04_But_Do_They_Really_Care_About_Us.md)*
