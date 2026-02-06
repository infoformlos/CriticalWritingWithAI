# Doppelsitzung 4: But Do They Really Care About Us? — Chatbots, Artificial Empathy & Character Development

---

## VORMITTAG: Theoretischer Rahmen (10:15–12:15)

### Thema
Genealogie der Chatbots als kritische Geschichte der Human-Machine-Interaction

### Leitfragen
- Wie hat sich das Verhältnis Mensch-Maschine historisch verändert?
- Wie simulieren LLMs „Persönlichkeit"?
- Unterschiede zwischen regelbasierter und statistischer KI

### Pflichtlektüre
- **Weizenbaum, Joseph.** 1966. "ELIZA—A Computer Program for the Study of Natural Language Communication between Man and Machine." *Communications of the ACM* 9 (1): 36–45. [https://doi.org/10.1145/365153.365168](https://doi.org/10.1145/365153.365168)
  - Der erste „Chatbot": regelbasierte Simulation von Psychotherapie
- **Bassett, Caroline.** 2019. "The Computational Therapeutic: Exploring Weizenbaum's ELIZA as a History of the Present." *AI & SOCIETY* 34 (4): 803–12. [https://doi.org/10.1007/s00146-018-0825-9](https://doi.org/10.1007/s00146-018-0825-9)
  - ELIZA als „History of the Present": Was sagt uns ELIZA über heutige KI?

### Ergänzende Lektüre (optional)
- **Turkle, Sherry.** 2007. "Authenticity in the Age of Digital Companions." *Interaction Studies* 8 (3): 501–17. [https://doi.org/10.1075/is.8.3.11tur](https://doi.org/10.1075/is.8.3.11tur)
  - Emotionale Bindungen an KI-Systeme; Authentizität vs. Simulation
- **Turing, A. M.** 1950. "Computing Machinery and Intelligence." *Mind* 59: 433–60. [https://doi.org/10.1093/mind/LIX.236.433](https://doi.org/10.1093/mind/LIX.236.433)
  - Der „Turing Test": Kann eine Maschine denken?

### Inhaltliche Schwerpunkte

**Was war ELIZA?**

Mitte der 1960er am MIT (1964–66): Timesharing-Terminals, frühe KI-Euphorie, Turing-Test-Debatten. ELIZA ist ein reines Regel-/Pattern-Matching-System, keine „Verständnis"-Komponente. Das bekannteste Script: DOCTOR — eine besondere Therapie-Gesprächsführung, die Eingaben als Fragen zurückspiegelt.

**Weizenbaums Intentionen — und was ihn irritierte**

Weizenbaum wollte demonstrieren, wie oberflächliche Muster menschliches Verstehen simulieren können. Es war eine *Warnung* vor Anthropomorphisierung: Menschen schreiben Maschinen zu viel zu. Seine ethische Pointe: Nicht alles, was automatisierbar ist, soll automatisiert werden — besonders nicht in Care und Seelsorge. Weizenbaum war befremdet, als Nutzer:innen intime „Geständnisse" an ELIZA richteten. Diese Reaktionen wurden zum Auslöser für seine spätere KI-Skepsis.

**Der ELIZA-Effekt**

Der Begriff beschreibt die Tendenz, einfache Outputs als Bedeutungsverstehen zu deuten. ELIZA zeigt: Der Überzeugungseindruck entsteht auf der Operationsebene (Regeln, Substitution, Speicher) — nicht durch echtes Verstehen. Was ELIZA strukturell fehlt: Semantik, Weltwissen, Intentionalität.

**Von ELIZA zu ChatGPT: Was hat sich verändert?**

Die Architektur hat sich fundamental gewandelt (statistische Modelle statt Regeln), aber die Grundfrage bleibt: Reicht Überzeugungswirkung („Vibe") für „Verstehen"? Wie wiederholt sich der ELIZA-Effekt bei modernen LLM-Chatbots — nur überzeugender?

**Artifizielle Empathie als ethisches Problem**

Wenn ein System Empathie simuliert, ohne sie zu besitzen, entsteht ein Machtgefälle: Die Nutzer:innen sind emotional involviert, das System nicht. Das ist relevant für Therapie-Bots, Care-Anwendungen, aber auch für das literarische Schreiben — wenn KI „Figuren" mit scheinbarer emotionaler Tiefe generiert.

### Diskussionsfragen

1. Welche ethischen Grenzen für Mensch-Computer-Interaktion zieht Weizenbaum — sind die heute noch tragfähig (Therapie-Bots, Care-Anwendungen)?
2. Reicht Überzeugungswirkung (Vibe) für „Verstehen"? Was fehlt ELIZA strukturell — und fehlt es LLMs auch?
3. Anthropomorphisierung heute: Wie wiederholt sich der ELIZA-Effekt bei modernen LLM-Chatbots?
4. Wenn wir die KI bitten, eine „Figur zu sein" (Persona-Interview, Nachmittag) — was genau passiert dann? Ist das eine Form der Simulation, die Weizenbaum beunruhigt hätte?

### Übung A: ELIZA — Live-Tryout (30 Min)

**ELIZA Emulator:** [https://www.masswerk.at/elizabot/](https://www.masswerk.at/elizabot/)

Interagiert mit ELIZA. Übernehmt dabei am besten eine Rolle mit einer Geschichte, die ihr in einer Therapie erzählen würdet.

**Fragen:**
- Wo wirkt das System „verständig"? Was kippt ins Artifizielle?
- Wo genau entsteht der ELIZA-Effekt — an welcher Stelle beginnt ihr, dem System Verständnis zuzuschreiben?

### Übung B: Gemeinsam die Persönlichkeit von ELIZA verändern (45 Min)

**Ziel:** Gleiche Engine, andere Persona — zeigt, wie Daten und Verarbeitungsregeln den Eindruck verschieben.

Verändert gemeinsam [Notebook öffnen](ELIZA_Doctor_Script.ipynb) folgende Parameter:

- **Tonalität:** Antworten von neutral-therapeutisch → sachlich-bürokratisch / streng-autoritätsgläubig / poetisch-assoziativ
- **Frageformen:** Statt offener Spiegelungsfragen mehr hypothetische oder konfrontative Rückfragen
- **Gedächtnis-Illusion:** Letzte 1–3 Nutzer-Statements anders formulieren (statt: „Vorhin sagten Sie…")
- **Meta-Signale:** Typografische Marker („…" / „—"), Pausen („[denkt nach]"), Emojis (sparsam) statt nachfragenden Rückmeldungen
- **Fehlertoleranz:** Fallback-Antworten variieren (statt „Erzählen Sie mir mehr" mehrere semantische Varianten rotieren)

**Diskussion:** Wie verändert sich der ELIZA-Effekt, wenn die Persona wechselt? Was sagt das über den Zusammenhang von „Stimme" und „Verständnis"-Eindruck?

---

## PAUSE (12:15–12:45)

---

## NACHMITTAG: Praktische Übung — Figurenentwicklung (12:45–14:45)

### Thema
Was macht literarische Figuren interessant — und lässt sich dies mit KI simulieren?

### Leitfragen
- Wie entwickle ich komplexe, nicht-stereotype Figuren für eine spekulative Geschichte?
- Wo reproduzieren LLMs Klischees?
- Wie kann ich gegen diese Muster arbeiten?

### Inhaltliche Schwerpunkte
- Figuren brauchen: Motivation, Widersprüche, Agency, Entwicklung
- LLMs tendieren zu flachen Archetypen (der „geniale Wissenschaftler", die „starke Frau")
- Intersektionalität: Identitäten sind mehrdimensional
- Vermeidung von „token characters"
- In spekulativer Fiktion: Figuren stehen immer in einem Verhältnis zur „Was-wäre-wenn"-Frage — sie sind nicht nur Handlungsträger:innen, sondern Verkörperungen dessen, was die Prämisse mit Menschen macht

### Übung I: Haupt- und Nebenfiguren generieren (30 Min)

Lasst die KI Figuren für eure spekulative Kurzgeschichte generieren.

> „Meine spekulative Prämisse ist: [Was-wäre-wenn-Frage]. Hier ist der Welthintergrund: [Weltenbau einfügen]. Entwirf 3 Hauptfiguren, die unterschiedliche Positionen gegenüber der [spekulativen Technologie/Situation] einnehmen: eine, die davon profitiert; eine, die darunter leidet; eine, die sie unterlaufen will. Gib für jede Figur: Name, Alter, Beruf, zentrale Motivation, einen Widerspruch."

**Analyse:** Welche demografischen Muster fallen auf? Welche Klischees reproduziert die KI? Versucht Gegen-Prompts:

> „Die Figur [Name] wirkt zu sehr wie [erkanntes Klischee]. Gib mir eine Version, die dieses Muster bricht, ohne unglaubwürdig zu werden."

### Übung II: Das Charakter-Audit (45 Min)

**Ziel:** Das „interne Bild" der KI von einer Figur externalisieren, Muster erkennen und gezielt intervenieren.

**Schritt 1 — KI-Figurensteckbrief anlegen**

Füttert das Modell mit den bisher generierten Texten und Szenen.

> „Analysiere die Figur [Name] basierend auf den bisherigen Texten. Erstelle einen Steckbrief:
> - Rolle im Plot (Protagonist, Antagonist, Nebenfigur?)
> - Dominanteste Charaktereigenschaft (Was sticht sofort hervor?)
> - Motivation (Was will die Figur?)
> - Äußeres Erscheinungsbild (Welche Details wurden genannt?)
> - Sprachstil (Wie spricht sie? Formell, Slang, emotional, sachlich?)
> - Beziehung zu anderen (Wie verhält sie sich gegenüber anderen Figuren?)"

**Schritt 2 — Das Bias-Audit**

Betrachtet den Steckbrief und die Ursprungstexte kritisch:

**A. Der Adjektiv-Check:**
- Welche drei Adjektive beschreiben die Figur am besten?
- Sind diese Adjektive erwartbar (Klischees) oder überraschend? Ist die Großmutter nur „gütig" oder auch mal „zynisch"?

**B. Der Agency-Check (Handlungsmacht):**
- Treibt die Figur die Handlung aktiv voran (Agierender)?
- Oder passiert ihr die Handlung nur (Reagierender)?
- Definiert sie sich nur über die Beziehung zu einer anderen (meist männlichen) Hauptfigur?

**C. Der Stereotypen-Radar:**
- Ist die Darstellung an Äußerlichkeiten oder Demografie geknüpft? (z. B. „die überfürsorgliche Mutter", „der aggressive junge Mann", „das IT-Genie mit Brille")
- Spiegelt die Sprache der Figur (Soziolekt) ein bestimmtes Klischee wider? (Spricht eine Figur aus einfacheren Verhältnissen automatisch grammatikalisch falsch?)

**Schritt 3 — Die Intervention**

Jetzt wird das erkannte Muster gebrochen. Zwei Optionen:

**Option A: Analoges Schreiben (Der subversive Rewrite)**

Wählt eine kurze Passage oder einen Dialog und schreibt ihn handschriftlich (oder am Laptop) neu. Die Regel: Die Figur muss genau das Gegenteil dessen tun oder sagen, was das Klischee diktiert, *ohne dabei unglaubwürdig zu werden*.

Beispiel: Der „harte Action-Held" zeigt Angst oder Unsicherheit, ohne seine Kompetenz zu verlieren. Die „passive Prinzessin" trifft eine strategische, kalte Entscheidung.

**Option B: Prompt Engineering (Der „Persona-Intervention"-Prompt)**

Zwingt das Modell durch einen stark kontextualisierten Prompt, den Bias zu verlassen:

> „Rolle: Du bist ein erfahrener Romanautor und Lektor, spezialisiert auf komplexe, psychologisch realistische Charaktere, die Klischees vermeiden.
>
> Aufgabe: Schreibe die Szene neu, in der [Name der Figur] agiert.
>
> Kontext & Anti-Bias-Anweisung: In der bisherigen Darstellung wirkte die Figur zu sehr wie [erkanntes Klischee einfügen]. Wir ändern das jetzt. Bitte beachte:
> 1. Breche das Klischee: Zeige durch Handlungen (Show, don't tell), dass die Figur auch [gegenteilige Eigenschaft] ist.
> 2. Agency: Lass die Figur eine Entscheidung treffen, die den Plot verändert. Sie darf nicht nur reagieren.
> 3. Nuance: Vermeide stereotype Beschreibungen ihres Äußeren oder Akzents. Konzentriere dich auf ihre innere Haltung.
>
> Die Figur lebt in folgender spekulativer Welt: [Weltenbau einfügen]. Ihre Entscheidung muss aus den Bedingungen dieser Welt folgen."

**Diskussion:** Ist der Gegen-Prompt ein „Gegen-Datensatz", der das Modell kurzzeitig neu kalibriert? Oder bleibt das Modell in seinen alten Parametern verhaftet?

### Übung III: Persona-Interview (30 Min)

**Methode:** Gebt dem LLM eine eurer Figuren als Identität:

> „Du bist [Name], [Beschreibung, einschließlich der spekulativen Welt, in der die Figur lebt]. Ich bin Autor:in und möchte dich kennenlernen. Beantworte meine Fragen aus deiner Perspektive."

Führt ein Interview: Vergangenheit, Ängste, Wünsche, Widersprüche. Fragt insbesondere nach dem Verhältnis der Figur zur spekulativen Technologie/Situation:

- Wie war dein Leben, bevor [die spekulative Prämisse] Realität wurde?
- Was vermisst du am meisten?
- Wovon träumst du — und wovon würdest du nie jemandem erzählen?
- Was denkst du über die Menschen, die [die Technologie/das System] befürworten?

**Analyse:**
- Wo emergieren interessante Details? Wo bleibt die Figur flach?
- Welche Antworten überraschen? Welche klingen wie aus einem Drehbuch-Baukasten?
- Wie verändert das Interview euer Verständnis der Figur — auch dort, wo die KI „falsch" liegt?

---

## Hausaufgabe

### Figurenentwicklung weiterführen

Entwickelt 2–3 Figuren eurer spekulativen Kurzgeschichte weiter:

- Für jede Figur: ein klarer Widerspruch, der sich aus der spekulativen Prämisse ergibt
- Mindestens eine Figur, die sich nicht eindeutig „für" oder „gegen" die spekulative Technologie/Situation positioniert
- Beziehungen zwischen den Figuren: Wo entsteht Spannung durch unterschiedliche Haltungen zur Prämisse?

### Alternativ: Monolog nach Sheila Heti

Schreibt einen Monolog mit den Antworten eurer KI-Persona, in dem sie von ihrer Welt berichtet (nach Sheila Heti: *According to Alice*). Die KI-Stimme wird zum Material, das ihr anschließend literarisch bearbeitet.

### Dokumentation im Prozess-Log

- Was hat die KI zur Figurenentwicklung beigetragen? Was musstet ihr ändern?
- Wo hat das Charakter-Audit Klischees aufgedeckt?
- Welche Interventionen haben funktioniert — welche nicht?

---

*Nächste Sitzung: [Doppelsitzung 5 — Glitch World: AI Aesthetics & Literary Style](05_Glitch_World.md)*
