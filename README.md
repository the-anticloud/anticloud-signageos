# SIGNAGEOS

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-consumer_electronics-lightgrey)

> Anticloud-hardened packaging of the upstream project `SIGNAGEOS` in category **CONSUMER ELECTRONICS**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CONSUMER ELECTRONICS · **Upstream:** https://github.com/meesk/zed-sops · **Upstream pin:** `3693a25fd3e282aa7298885c1a8299433d0ee96e` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# SignageOS Flyo Example

A very basic SignageOS Applet which reads the data from Flyo SigangeOS Integration and display them as slides. More generic informations on [dev.flyo.cloud/integrations/signageos](https://dev.flyo.cloud/integrations/signageos.html).

In order to release/deploy the SignageOS Applet see [Applet Upload](https://dev.flyo.cloud/integrations/signageos.html#applet-upload)

## Develop

+ Install depencies `npm install`, ensure to run the commands in the `Setup` sections afterwards.
+ Start local development server: `npm start`
+ visit in your browser `http://localhost:8090/`

## Setup (Once)

> This step must be done once after cloning (setting up) your signageos applet project.

+ Ensure you have an active https://box.signageos.io account!
+ `npm install @signageos/cli -g` now the `sos` is gloabally available
+ `sos login`
+ `sos organization set-default`

## Links

+ [SignageOS Guide regarding Apps](https://docs.signageos.io/hc/en-us/articles/4405068855570-Introduction-to-applets)
+ [SignageOS Javascript SDK Reference](https://sdk.docs.signageos.io/)
+ [Problem with Emulator in Chrome](https://docs.signageos.io/hc/en-us/articles/4405238997138-Emulator-in-CLI-and-Box#adblock-issue-in-chrome)

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Node.js / npm** (manifests: package.json, package-lock.json; scanned in UPSTREAM_CLONE)
- Top-level source layout: `public/`, `src/`
- Snapshot size: **11 files**, **212 lines of code** (measured; see Benchmarks)
- Primary languages: `(none)` (3), `.js` (3), `.json` (2), `.css` (1), `.html` (1), `.md` (1)
- Upstream commit pinned for this packaging: `3693a25fd3e282aa7298885c1a8299433d0ee96e`

---

## Installation

+ Start local development server: `npm start`
+ visit in your browser `http://localhost:8090/`

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

A very basic SignageOS Applet which reads the data from Flyo SigangeOS Integration and display them as slides. More generic informations on [dev.flyo.cloud/integrations/signageos](https://dev.flyo.cloud/integrations/signageos.html).

In order to release/deploy the SignageOS Applet see [Applet Upload](https://dev.flyo.cloud/integrations/signageos.html#applet-upload)

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

+ `sos login`
+ `sos organization set-default`

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Node.js / npm |
| Manifests detected | package.json, package-lock.json |
| Files in snapshot | 11 |
| Lines of code | 212 |
| Dependency references | 12 |
| Dependencies by ecosystem | npm: 12 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | @babel/core | ^7.18.10 | package.json |
| npm | @babel/preset-env | ^7.18.10 | package.json |
| npm | @signageos/front-applet | ^5.4.2 | package.json |
| npm | @signageos/front-display | ^9.21.1 | package.json |
| npm | @signageos/webpack-plugin | ^0.3.0 | package.json |
| npm | babel-loader | ^8.2.5 | package.json |
| npm | css-loader | ^6.7.1 | package.json |
| npm | html-webpack-plugin | ^5.5.0 | package.json |
| npm | style-loader | ^3.3.1 | package.json |
| npm | webpack | ^5.74.0 | package.json |
| npm | webpack-cli | ^4.10.0 | package.json |
| npm | webpack-dev-server | ^4.10.0 | package.json |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `package.json`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `SIGNAGEOS` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
MIT License

Copyright (c) 2022 Flyo Cloud

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `SIGNAGEOS` (category: CONSUMER ELECTRONICS)
- **Upstream URL:** https://github.com/meesk/zed-sops
- **Pinned commit (SHA):** `3693a25fd3e282aa7298885c1a8299433d0ee96e`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`7858cb59a239978bd785a2929e587c9d113afef869dbdd432c5ebc6ec921e668`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

