# AfyaClimate SafeBirth — bilingual guided demo

**Status: concept demonstration / offline prototype; not deployed clinical software.**

This repository packages the current, locally testable website demonstration for Ubuntu Afyalink's AfyaClimate SafeBirth concept. It is a self-contained HTML application with two user roles (mothers/families and frontline health workers), English/Kiswahili choices, preset heat-safety educational messages, typed-message keyword routing, and emergency signposting. It is NOT a live AI system, NOT connected to WhatsApp, NOT a medical service, and NOT clinical decision support. No real users or patients were recruited for validation, and no maternal or neonatal health impact has been measured.

## Quick start

Open `demo/index.html` with a current browser (Chrome, Edge or Firefox). No installation, server, credentials, or network required. Choose an audience, choose Kiswahili/English, and interact with the guided topics. Do not enter identifiable patient information.

## Automated checks

Run `python -m unittest discover -s tests -v` from this repository's root. Tests check the presence of key UI controls and disclaimers; they **do not** establish clinical safety or model accuracy.

## What exists today

- Responsive interactive website demonstration, no backend
- Two audience pathways and English/Kiswahili switch
- Predefined guidance + simple keyword routing, not trained AI
- Descriptive emergency prompts and warnings against reliance on the demo

## Planned, not yet implemented

- Clinician-reviewed and versioned health-knowledge corpus
- Official WhatsApp Business API integration with opt-in and withdrawal
- Safe uncertain/urgent-message routing with human support agreements
- Data minimization, access controls, audit trails and privacy review
- Bounded NLP for Kiswahili intent classification and verified content retrieval
- Health-worker facility task assignment, follow-up and service measurements
- Validation with clinical experts and consenting end users

## Open-source scope

MIT license applies to code in this repository. Brand marks, patient information (none is included), clinical text requiring independent review, and any third-party assets must be handled according to their own rights and review requirements before reuse. If future modules are introduced, contributions must document safety and licensing.

## Safeguarding

This demonstration must never be advertised as a live 24/7 medical chatbot. Emergency messages must encourage seeking immediate professional care; it cannot respond to emergencies, diagnose, treat, prescribe, or make clinical risk predictions. Before deployment, obtain local clinical, ethics, privacy and regulatory reviews. See `docs/SAFETY.md`.

## Project background and evidence

Ubuntu Afyalink has experience with real healthcare facility energy projects, which is distinct from this unvalidated SafeBirth prototype. See `docs/EVIDENCE.md`. More detail on project framing and proposed milestones is available in the UNICEF funding application submitted separately.
