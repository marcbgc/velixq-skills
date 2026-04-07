---
name: velixq-email-templates
description: >
  Professional HTML email template creation for Velixq Digital Agency.
  Use when creating client onboarding emails, follow-up sequences, lead
  notification emails, GHL email templates, proposal emails, or any
  business email communication. Produces responsive HTML emails with
  Velixq branding for use in GoHighLevel workflows.
---

# Velixq Email Templates Skill

## When to Use

- Client onboarding email after signing and paying setup fee
- Lead notification email to client when new inquiry arrives
- Follow-up email after cold call or meeting
- Proposal/offer email
- Monthly report email to client

---

## Email Design Rules

1. Max width 600px, centered with margin auto
2. Inline CSS only (Gmail strips style blocks)
3. Table-based layout for structure
4. Velixq colors: Primary #0f172a (dark navy), Accent #3b82f6 (blue), White #ffffff
5. Font stack: Arial, Helvetica, sans-serif
6. CTA button: solid background, padding 12px 24px, border-radius max 6px
7. Footer: always include sender name, company

---

## Template 1: Client Onboarding

Subject: "Willkommen bei Velixq – Ihre Website startet jetzt"

Use after client signs and pays setup fee. Replace [NAME], [EMAIL], [CALENDAR_LINK].

Structure:
- Dark navy header with Velixq branding
- White body with personalized greeting
- Bullet list of next steps (24h contact, 7 days delivery, preview link)
- Blue CTA button linking to calendar
- Light gray footer with legal info

---

## Template 2: Lead Notification

Subject: "Neue Anfrage von Ihrer Website"

Use in GHL Workflow triggered on form submission, sends to client.

GHL merge tags to use:
- Name: {{contact.full_name}}
- Phone: {{contact.phone}}
- Email: {{contact.email}}
- Message: {{contact.message}}

Key sections: Alert header, lead data table, green callback CTA, tip about 5-minute callback rule.

---

## Template 3: Follow-Up After Cold Call

Subject: "Ihre neue Website – kurzes Beispiel fuer [FIRMENNAME]"

Use 1-2 hours after a cold call where prospect showed interest.
Replace [NAME], [FIRMENNAME], [DEMO_URL], [TELEFON].

Key sections: Brief intro referencing the call, demo website link button, soft CTA for 15-min meeting.

---

## Placeholders Reference

| Placeholder | Replace with |
|---|---|
| [NAME] | Ansprechpartner Vorname |
| [FIRMENNAME] | Offizieller Firmenname |
| [EMAIL] | E-Mail des Empfaengers |
| [DEMO_URL] | Link zur Demo-Website (z.B. sanitherm.velixq.com) |
| [CALENDAR_LINK] | Calendly oder GHL Kalender Link |
| [TELEFON] | Deine Telefonnummer |

---

## GHL Integration

To use templates in GoHighLevel:
1. Sub-Account > Marketing > Emails > Templates > New Template > HTML Editor
2. Paste HTML, replace placeholders with GHL merge tags
3. Use in Workflow: Action "Send Email" > select template

Common GHL merge tags:
- {{contact.first_name}}, {{contact.full_name}}
- {{contact.phone}}, {{contact.email}}
- {{location.name}}, {{location.phone}}
