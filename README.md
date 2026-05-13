# Silent Intrusions Defense Lab

A browser-based, decision-driven cybersecurity lab for healthcare, IoMT, and incident response professionals. Play interactive scenarios tied to *[Silent Intrusions]([book-link](https://www.thriftbooks.com/w/silent-intrusions/54914342/item/83943229/?mkwid=%7cdc&pcrid=76897258815619&pkw=&pmt=be&slid=&product=83943229&plc=&pgrid=1230353765528421&ptaid=pla-4580496747872836&utm_source=bing&utm_medium=cpc&utm_campaign=Shopping+%7c+NEW+condition+books&utm_term=&utm_content=%7cdc%7cpcrid%7c76897258815619%7cpkw%7c%7cpmt%7cbe%7cproduct%7c83943229%7cslid%7c%7cpgrid%7c1230353765528421%7cptaid%7cpla-4580496747872836%7c&msclkid=4affdbf9e3701bdef476b1fd585f877a#idiq=83943229&edition=72831245))*, make high-pressure defensive calls, and learn how different roles navigate cyber crises.

## Features

- **Role-based perspectives**: SOC Analyst, Clinical Lead, CISO, Biomedical Engineer, Incident Commander, AI Governance Officer
- **Scenario-driven learning**: Healthcare IoMT attack chains, supply chain compromise, credential harvesting, detection evasion
- **Decision scoring**: Each choice shifts campaign pressure metrics (patient safety, network trust, evidence quality, threat pressure, team stress)
- **Clue console**: Optional guided investigation commands—use like a reference, not a hacking simulator
- **Campaign tracking**: Watch real-time impact of your decisions across multiple scenarios
- **Offline-capable**: Load once, works offline; browser storage saves progress
- **No login required**: Zero barriers to entry—just download and open

## Quick Start

1. **Download** `Silent_Intrusions_Defense_Lab.html`
2. **Open in any browser** (Chrome, Firefox, Safari, Edge)
3. **Choose a role** and start the recommended scenario
4. **Read each decision prompt**, make your call, and see how it moves the pressure meters
5. **Optional**: Use the console to ask for clues (e.g., "trace specter", "summarize risk")

No installation. No dependencies. Works on desktop, tablet, and mobile.

## How It Works

### Scenarios (Modules)

Each scenario presents a healthcare or supply-chain incident from a specific operational angle. Scenarios vary by:
- **Difficulty**: Beginner, Intermediate, Advanced
- **Duration**: 5–15 minutes
- **Decision points**: 7–12 choices per module
- **Category**: Detection, Containment, Triage, Recovery, Evidence

### Scoring & Pressure

Decisions are scored on a scale of 0–5 points:

| Score | Outcome | Impact |
|-------|---------|--------|
| 5 | **Strong** | Balances safety, evidence preservation, containment, team communication |
| 2–4 | **Partial** | Buys time but adds uncertainty or operational risk |
| 0–1 | **High risk** | Increases pressure, weakens forensics, isolates teams |

Campaign meters track across all scenarios:
- **Patient safety**: Availability of critical care systems
- **Network trust**: Confidence in device/network integrity  
- **Evidence quality**: Forensic completeness for incident response
- **Threat pressure**: Active attacker capability and persistence
- **Team stress**: Burnout and decision-making clarity

### Role Lenses

Each role sees the same incident through a different lens:

- **SOC Analyst** → Signal clarity, containment speed, forensic evidence
- **Clinical Lead** → Patient safety first, care continuity, minimal disruption
- **CISO** → Cadence, accountability, enterprise risk governance
- **Biomedical Engineer** → Device firmware, physical custody, sensor telemetry validation
- **Incident Commander** → Named tradeoffs, clear ownership, time-boxed decisions
- **AI Governance Officer** → Authenticity of artifacts, synthetic data risk, reproducibility

Same scenario; different pressure points.

### Learning Sections

Companion articles explain real-world parallels for each threat:
- IoMT architecture weaknesses (wireless staging, firmware distribution)
- Supply chain attack vectors (trusted integrator compromise, signed malware)
- Detection strategies (behavioral baselines, anomaly thresholds)
- Role responsibilities under pressure

## No Prerequisites

This lab is a **standalone HTML file**. It contains:
- All scenario data (modules, decision trees, scoring)
- Learning content
- Visual assets (inline)
- Game state management (browser localStorage)

**Browser support**: Modern browsers (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+). Mobile-friendly.

## Offline Use

The lab loads fully in-browser. After initial load:
- Works offline
- Saves progress to browser storage automatically
- No network calls after load

⚠️ **Storage note**: If you clear browser cache/cookies, progress is lost. Encourage users to finish scenarios in one session or implement a download/export feature if persistence is critical.

## Customization & Deployment

### Self-hosted

1. Place `Silent_Intrusions_Defense_Lab.html` on a web server or CDN
2. Share a direct link; users download or open in-browser
3. No build step required

### Embedding

Embed in a learning platform (LMS, training portal):
- Add as an iframe
- Keep same origin if storing progress server-side
- No external dependencies

### Extending

To add new scenarios or learning sections, edit the JavaScript data structures in the HTML:

```javascript
// Add to modules array
const newModule = {
  id: 'supply_chain_04',
  title: 'Firmware Trust Boundary Breach',
  subtitle: 'A trusted integrator's build pipeline is compromised.',
  category: 'Supply Chain',
  difficulty: 'Advanced',
  minutes: 12,
  steps: [ /* decision tree */ ],
  artifacts: [ /* clues */ ],
  commands: { /* console commands */ },
  roleGuidance: { /* role-specific context */ }
};

// Add to learningSections array
const newLearning = {
  id: 'fw_supply_chain',
  title: 'Firmware Distribution & Trust',
  body: 'Real-world example...'
};
```

## Files in This Repository

- `Silent_Intrusions_Defense_Lab.html` — The complete, self-contained lab

---

**No login. No install. Starts in seconds. Works offline.**

Start with the recommended scenario, or browse the catalog. Choose your role and see how your decisions move the pressure meter.

## Related Resources

- **[Silent Intrusions](https://www.thriftbooks.com/w/silent-intrusions/54914342/item/83943229/?mkwid=%7cdc&pcrid=76897258815619&pkw=&pmt=be&slid=&product=83943229&plc=&pgrid=1230353765528421&ptaid=pla-4580496747872836&utm_source=bing&utm_medium=cpc&utm_campaign=Shopping+%7c+NEW+condition+books&utm_term=&utm_content=%7cdc%7cpcrid%7c76897258815619%7cpkw%7c%7cpmt%7cbe%7cproduct%7c83943229%7cslid%7c%7cpgrid%7c1230353765528421%7cptaid%7cpla-4580496747872836%7c&msclkid=4affdbf9e3701bdef476b1fd585f877a#idiq=83943229&edition=72831245)** — The accompanying book by John Chirillo
- **[Connection Security Services]([https://www.connection.com/](https://www.connection.com/solutions-services/cybersecurity)** — External Link to Connection's Professional, Advisory, and Managed Security Services
