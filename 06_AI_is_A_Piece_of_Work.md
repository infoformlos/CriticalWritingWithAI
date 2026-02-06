# Doppelsitzung 6: AI is A Piece of Work — Resources & The Labour of Authorship

---

## VORMITTAG: Materialität Künstlicher Intelligenz (10:15–12:15)

### Thema
Ressourcenverbrauch und Lieferketten der KI

### Leitfragen
- Welche materiellen Ressourcen braucht KI?
- Wer leistet die unsichtbare Arbeit hinter KI-Systemen?
- Was bedeutet „verantwortungsvolle Nutzung"?

### Pflichtlektüre
- **Crawford, Kate.** 2021. *Atlas of AI: Power, Politics, and the Planetary Costs of Artificial Intelligence.* New Haven: Yale University Press.
  - Lesen: Introduction + Kapitel "Earth" + Kapitel "Labor"
  - Umfassende Analyse der materiellen, ökologischen und sozialen Kosten von KI
- **Perrigo, Billy.** 2023. "OpenAI Used Kenyan Workers on Less Than $2 Per Hour to Make ChatGPT Less Toxic." *TIME*, January 18, 2023.
  - Investigative Reportage zu Content-Moderation als ausbeuterische Arbeit

### Ergänzende Lektüre (optional)
- **Newlands, Gemma.** 2021. "Lifting the Curtain: Strategic Visibility of Human Labour in AI-as-a-Service." *Big Data & Society* 8 (1): 1–14. [https://doi.org/10.1177/2053951721997366](https://doi.org/10.1177/2053951721997366)
  - Unsichtbare menschliche Arbeit hinter „automatisierten" Systemen
- **Joler, Vladan, and Kate Crawford.** 2018. "Anatomy of an AI System: The Amazon Echo as an Anatomical Map of Human Labor, Data and Planetary Resources." [http://www.anatomyof.ai](http://www.anatomyof.ai)
  - Visuelles Diagramm der kompletten Lieferkette eines AI-Systems
- **Penn, Jonnie.** 2023. "Animo Nullius." In: Ali et al., "Histories of Artificial Intelligence: A Genealogy of Power." *BJHS Themes* 8.
  - Penns Begriff *animo nullius* („Niemands Geist") beschreibt, wie die Aneignung von Daten als „Entdeckung" naturalisiert wird — analog zu *terra nullius* in der kolonialen Landnahme

### Inhaltliche Schwerpunkte

**Planetare Kosten**

KI existiert nicht in einer „Cloud", sondern in physischen Gebäuden mit konkretem Verbrauch:
- Wasserverbrauch für Serverkühlung (z. B. ~50–100 ml Wasser pro GPT-4-Anfrage)
- CO₂-Emissionen (Training von GPT-3: ~550 Tonnen CO₂)
- Seltene Erden für Prozessoren (Kobalt, Lithium)

**Arbeit**

Hinter jedem LLM stehen mehrere Schichten menschlicher Arbeit:
- Data-Annotation & Labeling (oft im Globalen Süden, Niedriglohn)
- Content-Moderation (traumatisierende Arbeit, $2/Stunde — Perrigo)
- Ingenieur:innen & Forscher:innen (hochbezahlt, meist im Globalen Norden)

Crawford nennt dies die „Anatomie" eines KI-Systems: Vom Bergbau über die Chip-Produktion bis zur Clickwork-Annotation reicht eine globale Lieferkette, die systematisch unsichtbar gemacht wird.

**Datenkolonialismus (Penn)**

Penn zieht Parallelen zwischen *terra nullius* (koloniale Landnahme) und der heutigen Aneignung des „Data Commons" durch Tech-Konzerne. Der Begriff *animo nullius* beschreibt, wie die Nutzung von „Geist-als-Computer"-Metaphern die Extraktion von Daten als wissenschaftlichen Fortschritt legitimiert. Große Sprachmodelle werden als Vermögenswerte (Assets) behandelt, die durch Rentenökonomie (Cloud-Abonnements) Gewinne generieren, während die Urheberschaft der Trainingsdaten verschleiert wird.

**Geopolitik**

- Chip-Produktion (Taiwan, Südkorea)
- Dateninfrastruktur (Server-Farmen in USA, EU, China)
- Regulierung (EU AI Act, Chinas Algorithm Governance)

**Rückbezug zum Seminar**

Wir haben ein Semester lang mit KI geschrieben. Jede Prompt-Anfrage, jede Iteration, jedes Brainstorming hat Ressourcen verbraucht — Energie, Wasser, menschliche Arbeit. Diese Sitzung macht die materiellen Bedingungen dessen sichtbar, was wir getan haben.

### Übung: Anatomie eines LLMs — Gruppenarbeit (60 Min)

Vier Gruppen recherchieren jeweils einen Aspekt der materiellen Infrastruktur hinter dem LLM, mit dem ihr im Seminar gearbeitet habt:

**Gruppe 1: Data-Annotation & Click-Work**
- Wer hat die Trainingsdaten annotiert? Unter welchen Bedingungen?
- Was ist „Ghost Work" (Mary Gray / Siddharth Suri)?

**Gruppe 2: Server-Standorte & Energieverbrauch**
- Wo stehen die Server? (Google: Hanau, Saint-Ghislain; OpenAI/Microsoft: „Stargate"-Projekt, Abilene/Texas)
- Welche Probleme der Wasser- und Energieversorgung gibt es an diesen Standorten?

**Gruppe 3: Content-Moderation als Arbeit**
- Was genau tun Content-Moderator:innen? (Bezug zu Perrigo)
- Welche psychischen Folgen hat diese Arbeit?
- Wie verhalten sich die Arbeitsbedingungen zu dem, was wir als „hilfreiche" und „sichere" KI erleben?

**Gruppe 4: Geopolitik & Lieferketten**
- Woher kommen die Rohstoffe für die Chips?
- Welche geopolitischen Abhängigkeiten bestehen?
- Welche Regulierungsansätze gibt es (EU AI Act, etc.)?

**Präsentationen:** Jede Gruppe 5 Minuten.
**Referenz:** Joler & Crawford „Anatomy of an AI System" als visuelles Modell.

### Übung: Ein Prompt und sein Ressourcenverbrauch (30 Min)

**Arbeitsblatt** (wird ausgeteilt)

**Schritt 1 — Prompt auswählen**

Wählt einen Prompt aus eurer spekulativen Kurzgeschichte. Notiert ihn und schätzt seine Komplexität ein.

- Ungefähre Token-Länge berechnen über: [OpenAI Tokenizer](https://platform.openai.com/tokenizer)
- Einbeziehen: Chain-of-thought (Kontextmaterial im Chat), Zusatzmaterial

**Schritt 2 — Fußabdruck berechnen**

Nutzt folgende Schätzwerte:

*A. Energieverbrauch:*
Ungefähren Energieverbrauch berechnen über: [EcoLogits Calculator (Hugging Face)](https://huggingface.co/spaces/genai-impact/ecologits-calculator)

*B. Wasserverbrauch:*
- Durchschnitt (2025/26): ~50–100 ml Wasser pro GPT-4-Anfrage
- Hocheffiziente Modelle: ~0,26 ml pro Prompt

**Schritt 3 — Recherche: Wo „arbeitet" eure KI?**

Findet heraus, wo die Rechenleistung für euer Modell wahrscheinlich herkommt:
- Google (Gemini): [datacenters.google](https://datacenters.google) — Standorte wie Hanau (DE), Saint-Ghislain (BE), Council Bluffs (USA)
- OpenAI/Microsoft (GPT-4): „Stargate"-Projekt — Abilene (Texas), New Mexico

**Diskussion:**
- Welche ethischen Verpflichtungen haben wir als Nutzer:innen?
- Wie verändert das Wissen um den Ressourcenverbrauch euer Verhältnis zum eigenen Schreibprozess?
- Ist der Energie- und Wasserverbrauch ein moderner Ausdruck von *terra nullius* — die Annahme, natürliche Ressourcen stünden zur freien Ausbeutung bereit?

---

## PAUSE (12:15–12:45)

---

## NACHMITTAG: Präsentationen & Abschlussreflexion (12:45–14:45)

### Format: Textpräsentationen

Jede:r präsentiert (8–10 Min pro Person):

**1. Textausschnitt vorlesen (2–3 Seiten)**

Lest eine Schlüsselpassage eurer spekulativen Kurzgeschichte vor — die Stelle, die eure „Was-wäre-wenn"-Frage am stärksten verdichtet.

**2. Prozess-Reflexion (3–5 Min)**

- Was war deine „Was-wäre-wenn"-Frage?
- Wie hast du KI genutzt? (Brainstorming, Worldbuilding, Figuren, Plot, Stil)
- Wo musstest du gegen das Modell arbeiten?
- Was war überraschend? Was frustrierend? Was produktiv?

**3. Diskussion (2–3 Min)**

- Peer-Feedback: Was funktioniert gut? Welche Überarbeitungen könnten noch gemacht werden?

### Gemeinsame Abschlussreflexion

**Autorschaft**
- Was hat „Autorschaft" in diesem Seminar bedeutet?
- Ist der Text „mein" Text, wenn KI daran mitgeschrieben hat?
- Wo verläuft die Grenze zwischen Tool und Co-Autor:in?
- Autorschaft als ästhetische Arbeit: Auswahl, Überarbeitung, Entscheidung gegen den Default

**Spekulative Fiktion als Technikkritik**
- Ist spekulative Fiktion tatsächlich ein Werkzeug zur Technikkritik?
- Was haben wir durch das Schreiben *über* KI *mit* KI gelernt?
- Hat das fiktionale Denken neue Perspektiven auf die Technologie eröffnet?

**Kritische Praktiken**
- Welche kritischen Praktiken haben wir entwickelt?
  - Bias-Audits, Gegen-Prompts, Constraint-Prompting, manuelle Überarbeitung
  - Reflexion auf Materialität und Arbeit
  - Datensatz-Analyse als Methode der Technikkritik
- Wie positionieren wir uns zu KI im literarischen Feld?

**Paratexte & Transparenz — Best Practices gemeinsam entwickeln**

Zum Abschluss entwickeln wir gemeinsam Vorschläge für die Kennzeichnung von KI-unterstützten Texten:

- „Dieser Text wurde mit Unterstützung von [Modell, Version] entwickelt."
- „KI wurde für [spezifische Aufgaben] genutzt, z. B. Brainstorming, Weltenbau."
- „Alle finalen stilistischen Entscheidungen wurden manuell getroffen."

---

## Abgabe: Textmappe (15. März 2026)

### Bestandteile

1. **Spekulative Kurzgeschichte** (6–10 Seiten)
2. **Prozess-Log** (dokumentierte Prompts, Entscheidungen, Iterationen)
3. **Reflektierende Einordnung** mit Bezug auf die im Seminar rezipierten theoretischen Texte (3–5 Seiten, mindestens 5 Texte substantiell einbezogen)
4. **Appendix:** Der generierte und/oder selbst überarbeitete Text mit Kennzeichnung der KI-Anteile

### Bewertungskriterien

**Prozess-Dokumentation (30%)**
- Vollständigkeit des Prompt-Logs
- Reflexionstiefe (nicht nur „Was?", sondern „Warum?")
- Nachvollziehbarkeit der Entscheidungen
- Kritische Auseinandersetzung mit Grenzen der Technologie

**Kritische Auseinandersetzung mit Theorie (30%)**
- Theoretische Fundierung der reflektierenden Einordnung
- Bezug auf Seminartexte
- Eigenständige Argumentation (nicht nur Zusammenfassung)
- Kritische Perspektive auf eigene Praxis

**Kreative Ergebnisse (20%)**
- Narrative Qualität der Kurzgeschichte
- Umsetzung der „Was-wäre-wenn"-Frage
- Kritisches Potenzial (Sichtbarmachung von Machtverhältnissen)
- Stil & Originalität (Abweichung von generischen Mustern)
- Konsistenz (Weltenbau, Figuren, Plot)

**Seminarbeteiligung (20%)**
- Qualität der Präsentationen
- Konstruktive Diskussionsbeiträge
- Peer-Feedback
- Anwesenheit und aktive Mitarbeit

---

*[Zurück zur Übersicht](README.md)*
