# Electronics Design & Simulation - EDA Work Samples

![Scope](https://img.shields.io/badge/scope-self--directed-0F766E?style=flat-square)
![Focus](https://img.shields.io/badge/focus-EDA%20%2B%20simulation-2563EB?style=flat-square)
![Tools](https://img.shields.io/badge/tools-KiCad%20%7C%20LibrePCB%20%7C%20Ngspice%20%7C%20Qucs--S-7C3AED?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-475569?style=flat-square)

This repository is a self-directed portfolio of electronics design and simulation work samples. It shows how I document circuit behavior, review schematic and PCB workflows, and evaluate AI-generated EDA content with an emphasis on correctness, reproducibility, and explicit assumptions. It is not client work, not a manufactured product set, and not proof of physical board validation.

## Portfolio Snapshot

<table>
  <tr>
    <td valign="top" width="33%">
      <strong>Simulation</strong><br>
      RC low-pass filter in ngspice<br>
      AC source, resistor, capacitor, and ground<br>
      Cutoff frequency and frequency-response review
    </td>
    <td valign="top" width="33%">
      <strong>Workflow</strong><br>
      555 timer LED blinker<br>
      KiCad schematic flow, ERC, DRC, and footprints<br>
      PCB layout and Gerber generation notes
    </td>
    <td valign="top" width="33%">
      <strong>Review</strong><br>
      EDA AI output quality review<br>
      Find flaws, rewrite instructions, and verify assumptions<br>
      Reproducible evaluation checklist
    </td>
  </tr>
</table>

The diagram below shows how the repository is organized around simulation, workflow review, and AI-output evaluation.

```mermaid
flowchart TB
    A[EDA work-sample portfolio] --> B[Simulation track]
    A --> C[Workflow track]
    A --> D[Review track]

    B --> B1[RC low-pass filter]
    B --> B2[ngspice netlist]
    B --> B3[Expected results]

    C --> C1[555 timer LED blinker]
    C --> C2[KiCad ERC and DRC]
    C --> C3[Footprints and Gerbers]

    D --> D1[Flawed AI answer]
    D --> D2[Review findings]
    D --> D3[Improved answer]

    classDef root fill:#111827,stroke:#111827,color:#FFFFFF;
    classDef sim fill:#E8F7EE,stroke:#2E7D32,color:#111111;
    classDef workflow fill:#FFF4E5,stroke:#C47F00,color:#111111;
    classDef review fill:#FDECF4,stroke:#A61B55,color:#111111;
    class A root;
    class B,B1,B2,B3 sim;
    class C,C1,C2,C3 workflow;
    class D,D1,D2,D3 review;
```

## About

Description: this is a self-directed EDA work-sample portfolio focused on circuit simulation documentation, schematic and PCB workflow review, and AI-output evaluation.

The goal of this portfolio is to show how I approach electronics tasks with the same discipline I use in software engineering: clear requirements, explicit assumptions, reproducible steps, and structured review. Each sample is built to be readable on its own and to demonstrate how I think about a circuit from the brief, through the simulation or workflow steps, to the documented result and limitations.

These samples focus on basic analog simulation, schematic and PCB workflow understanding, BOM documentation, ERC and DRC awareness, and critical evaluation of AI-generated EDA content. The intent is to demonstrate EDA literacy and disciplined documentation, not to claim senior electrical engineering experience or fabricated hardware validation.

## Tools Referenced

| Tool | Role in this portfolio |
| --- | --- |
| KiCad | Schematic capture, footprint assignment, PCB layout review, ERC/DRC awareness |
| LibrePCB | Alternative EDA workflow reference for schematic and board organization |
| Ngspice | Netlist-based circuit simulation and frequency-response review |
| Qucs-S | GUI-oriented circuit simulation reference and result interpretation |

## Skills Demonstrated

- Circuit simulation documentation
- SPICE netlist interpretation
- Schematic workflow understanding
- Basic PCB design review concepts
- Component and BOM documentation
- ERC and DRC awareness
- AI-generated EDA output evaluation
- Reproducible technical documentation

## Projects

| Project | Focus | Key Files |
| --- | --- | --- |
| [RC Low-Pass Filter in ngspice](projects/01-rc-low-pass-filter-ngspice/README.md) | Beginner-friendly analog simulation and frequency-response interpretation | `rc-low-pass.cir`, `expected-results.md`, `quality-checklist.md` |
| [555 Timer LED Blinker](projects/02-555-timer-led-blinker/README.md) | Conceptual KiCad workflow, BOM planning, and simulation vs hardware boundaries | `schematic-workflow.md`, `simulation-notes.md`, `bill-of-materials.md`, `limitations.md` |
| [EDA AI Output Quality Review](projects/03-eda-ai-output-quality-review/README.md) | Reviewing flawed AI-generated EDA instructions and rewriting them clearly | `fake-ai-generated-answer.md`, `review-findings.md`, `improved-answer.md`, `evaluation-checklist.md` |

## Why This Helps With AI And EDA Asset Evaluation

This repository is also meant to support AI research and EDA asset evaluation work. The examples show how I inspect output for missing units, missing ground references, unclear simulator assumptions, absent validation steps, and overconfident claims that simulation alone proves a working PCB. That review mindset is useful when judging generated technical content for correctness, reproducibility, and safety.

## GitHub

- GitHub: https://github.com/onehermes

## Notes

- No claim is made here of senior electrical engineering experience.
- No fabricated PCB manufacturing, lab testing, or reliability validation is presented.
- The focus is on clarity, discipline, and reproducible documentation.
