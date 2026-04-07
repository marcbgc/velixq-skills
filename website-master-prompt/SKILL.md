---
name: website-master-prompt
description: >
  Website Master Prompt for Velixq Digital Agency. Use when the user wants to
  create a detailed project briefing for a new website task. Guides through
  5 essential questions (Context, Role, Examples, Output Format, Approach)
  and generates one perfect structured prompt. Trigger when user says
  "briefing", "neues Projekt", "Website erstellen fuer Kunde", or asks
  to prepare a task prompt.
---

# Website Master Prompt

This skill guides the creation of a perfect Manus briefing for website projects.
It asks 5 questions one at a time and generates a final structured prompt.

## When to Use

Trigger this skill when the user wants to:
- Start a new website project for a client
- Create a detailed briefing before building
- Ensure nothing is forgotten before execution

## The 5-Question Framework

Ask these questions ONE AT A TIME. Wait for the answer before asking the next.

### Question 1 – Context (Hintergrund)
"Was ist der Hintergrund des Projekts? Wer ist der Kunde, was macht er, wer ist seine Zielgruppe, und was ist das Ziel der Website?"

### Question 2 – Role (Rolle)
"Welche Rolle soll ich fuer diese Aufgabe einnehmen? (z.B. Senior Web Designer, Conversion-Experte, Brand Designer fuer Handwerksbetriebe)"

### Question 3 – Examples (Beispiele)
"Gibt es 1-2 Referenz-Websites oder Stil-Beispiele die dir gefallen? Oder beschreib den gewuenschten Look: modern/minimalistisch, dunkel/hell, luxurioees/handwerklich, etc."

### Question 4 – Output Format (Format)
"Wie soll das Ergebnis aussehen? (z.B. fertige React-Website, HTML/CSS, Anzahl Sektionen, welche Seiten: Home/Ueber uns/Kontakt, etc.)"

### Question 5 – Approach (Herangehensweise)
"Gibt es besondere Anforderungen oder Einschraenkungen? (z.B. Farben der Firma, Logo vorhanden, spezifische Inhalte, GHL-Formular einbinden, bestimmte Sprache)"

## Final Prompt Generation

After all 5 answers, generate ONE structured prompt using this template:

---
TEMPLATE:
Du bist [ROLLE] mit Expertise in [BEREICH].

PROJEKT-KONTEXT:
[HINTERGRUND aus Antwort 1]

ZIELGRUPPE:
[Zielgruppe aus Antwort 1]

AUFGABE:
Erstelle eine professionelle, außergewoehnliche Website fuer [KUNDENNAME].

DESIGN-ANFORDERUNGEN:
- Stil: [aus Antwort 3]
- Referenzen: [aus Antwort 3]
- Besonderheiten: [aus Antwort 5]

TECHNISCHE ANFORDERUNGEN:
- Format: [aus Antwort 4]
- Sektionen: [aus Antwort 4]

VELIXQ STANDARDS (immer einhalten):
- Mobile-first, responsive Design
- Impressum & Datenschutz Sektion
- Kontaktformular (GHL-ready)
- Ladezeit optimiert
- Keine generischen AI-Aesthetics (kein Inter-Font, keine lila Gradienten)

Denke Schritt fuer Schritt: Plane zuerst die Struktur und das Design-Konzept,
dann implementiere es. Erklaere kurz deine Design-Entscheidungen.
---

## Important Rules

- NEVER ask all 5 questions at once
- Always wait for the answer before asking the next question
- Keep questions short and concrete
- After generating the final prompt, tell the user: "Kopiere diesen Prompt und starte einen neuen Task damit."
