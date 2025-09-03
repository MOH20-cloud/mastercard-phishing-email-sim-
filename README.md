# Mastercard Forage — Phishing Email Simulation (Task-1)

This repo contains my deliverable for **Task One** of the Mastercard Virtual Experience Program on Forage: craft a believable phishing email simulation to raise employee awareness.

##  What I produced
- A realistic (but **safe**) training email designed to encourage a click **for simulation purposes**.
- Context is tailored to a Mastercard employee; link is masked within natural text; grammar and tone are professional; legitimacy points (ticket #, time window, contact, footer) are included.

>  Note: The URL in this simulation points to a **training placeholder** (`https://training.example.com/mc/sso/verify`). No real credentials are collected.

---

## ✉️ Phishing Simulation Email 

```
From: IT Service Desk | Mastercard <service-desk@mastercard.com>
To: ismail.muhammad@mastercard.com
Subject: Action required: SSO session reset for your account – complete by 5:00 PM ET today

Hi ismail,

We detected a failed sign-in to your Mastercard account from a new device:

  • Location: Charlotte, NC
  • Time: 9:14 AM 
  • Browser: Chrome 126
  • IP: 23.54.88.12
  • Ticket: MC-487216

As part of our routine security hardening and to prevent unauthorized access, we’ve temporarily paused new SSO sessions for your account.

Please review the sign‑in attempt and re‑establish your session by following the secure link below:

  Review activity & reset session: https://training.example.com/mc/sso/verify

If you recognize this activity, you’ll be asked to refresh your session. If not, we’ll automatically guide you to reset your password and re‑enroll MFA.

This link will expire at 5:00 PM ET today. If you need assistance, call the Service Desk at +1‑800‑555‑0199 and reference Ticket MC-487216.

Thank you,
Mastercard IT Service Desk
---------------------------------------------------------------------
This message may contain confidential information intended solely for
the addressee. If you received it in error, please delete it and
notify the Service Desk.

```

---

## Why this works (social engineering rationale)

- **Urgency & specificity**: A concrete deadline (“by 5:00 PM ET”) and a specific ticket number drive action.
- **Legitimacy signals**: Service Desk branding, a phone number, and a standard confidentiality footer reduce suspicion.
- **Familiar workflow**: References to SSO, MFA, and session reset mirror real internal processes.
- **Masked, natural link text**: The call‑to‑action is embedded in a sentence, not a naked URL.
- **Benign telemetry**: Location, time, browser, and IP details feel like automated security alerts.

## Red flags employees should learn to spot

- **Sender domain**: Always verify the sending domain and the “envelope” sender.
- **Hover over links**: Check the actual destination before clicking.
- **Urgency pressure**: Time‑boxed demands are a common manipulation tactic.
- **Unexpected security alerts**: Validate via your usual IT channels when in doubt.

## How I would operationalize this as a simulation

- Send to a small pilot group with an allow‑listed training URL.
- Track metrics: delivery, open rate, click‑through, report rate.
- Auto‑redirect clicks to a 60‑second micro‑training page (what to check next time).
- Share an anonymized summary with lessons learned.

## Repo Structure

```
mastercard-forage-phishing-sim/
├─ README.md
├─ phishing_email_v1.md
├─ indicators_and_training.md
├─ LICENSE
└─ .gitignore
```

