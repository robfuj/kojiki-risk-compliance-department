# Bots of Risk / Compliance  (docx S5 candidate menu)

These are the **Major sub-functions** of Risk / Compliance from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 8.

- `enterprise-risk` — **Enterprise Risk**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `operational-risk` — **Operational Risk**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `financial-risk` — **Financial Risk**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `regulatory-compliance` — **Regulatory Compliance**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `aml-kyc` — **AML/KYC**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `monitoring` — **Monitoring**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `testing` — **Testing**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
- `risk-governance` — **Risk Governance**  ·  titles: Chief Risk Officer, Chief Compliance Officer, Head of Compliance, Risk Director, Compliance Director, Compliance Officer, AML Officer, Risk Analyst
