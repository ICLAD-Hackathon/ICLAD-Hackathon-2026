# ICLAD Hackathon 2026

This repository is the top-level entry point for the ICLAD-DAC 2026 GenAI Chip
Hackathon problem repositories. The hackathon asks teams to use generative AI to
solve chip design tasks across the RTL-to-GDSII flow, including RTL design,
verification, optimization, and physical design.

For event details, registration, schedule, and prize eligibility, see the
[official ICLAD hackathon page](https://iclad.ai/hackathon).

## Problem Repositories

Participants may attempt any one problem category or multiple problem
categories.

| Problem category | Repository | Summary |
| --- | --- | --- |
| NVIDIA problems | [ICLAD26-NVIDIA-Problems](./problem-categories/ICLAD26-NVIDIA-Problems) | RTL optimization tasks for IPs such as asynchronous FIFO, SHA-512, NVDLA, and selected OpenTitan blocks. Solutions are evaluated for functional correctness and power, performance, area, timing, and model-usage metrics. |
| NXP problems | [ICLAD26-NXP-Problems](./problem-categories/ICLAD26-NXP-Problems) | SoC RTL generation tasks where agents infer specifications from architecture diagrams, generate Verilog with the provided RTL generation library, integrate IP blocks, and pass simulation tests. |
| ASU problems | [ICLAD26-ASU-Problems](./problem-categories/ICLAD26-ASU-Problems) | DRC fixing tasks where agents repair ASAP7 KLayout Python layout scripts using DRC reports, design rules, screenshots, and connectivity references. |

The problem repositories are included here as git submodules. To clone this
repository with all problem folders populated, use:

```bash
git clone --recurse-submodules <repo-url>
```

If you already cloned the repository, initialize the submodules with:

```bash
git submodule update --init --recursive
```

## Tracks

The hackathon has two participation tracks:

| Track | Description |
| --- | --- |
| On-Prem Track | Teams use resource-constrained local models, including small language models running on laptops. This track is primarily an in-person DAC competition, with preparation resources provided before DAC. |
| Cloud Track | Teams may use cloud-hosted models, including large-scale LLMs. This track includes a pre-DAC online phase and an in-person DAC phase. |

Participants may compete in the On-Prem Track, the Cloud Track, or both tracks.
They may also attempt one problem category or multiple problem categories.

## Infrastructure

### Cloud Track

Cloud Track agents will be available through Vertex AI, and final evaluation
will run on Google Cloud Platform (GCP). Participants will receive GCP accounts
one week before the in-person phase. Until then, teams may use their own
resources to develop agents offline, but final evaluation will use Vertex AI and
Gemini models.

For evaluation, sandbox environments will be set up to prevent other agents or
unrelated processes from running during benchmark execution. Example Vertex AI
setup instructions for the Cloud Track are available in each problem category
repository.

### On-Prem Track

The On-Prem Track uses local, resource-constrained models. Participants will get
access to Qualcomm Developer Cloud (QDC) to prepare; QDC access details will be
provided soon.

On the day of DAC, participants will receive laptops for the in-person contest
and may continue development on those machines. The On-Prem Track contest will
take place only in person.

### Scoring

Scoring is defined by each problem category. Evaluation will include token
counts and the problem-specific criteria described in the corresponding problem
repository.

## Registered Participants

Registered teams will be listed here with the team name and primary member
affiliation.

| Team name | Primary member affiliation |
| --- | --- |
| TBD | TBD |

## Awards

One award will be given per track per problem category:

| Problem category | On-Prem Track | Cloud Track |
| --- | --- | --- |
| NVIDIA problems | 1 award | 1 award |
| NXP problems | 1 award | 1 award |
| ASU problems | 1 award | 1 award |

This gives a total of 6 awards.

## Important Participation Notes

- In-person participation at DAC 2026 in Long Beach on Sunday, July 26, 2026 is
  required for prize eligibility.
- Participants must have DAC or I LOVE DAC access for the in-person event.
- Hidden benchmark problems or hidden test cases may be introduced in person on
  the day of DAC.
- Scoring details are problem-specific; see each problem repository for setup,
  agent interface, execution, and evaluation instructions.

## Contact Us

For questions, contact:

iclad2025-hackathon@googlegroups.com

## Acknowledgements

We thank Qualcomm for sponsorship and Google for providing GCP accounts.
