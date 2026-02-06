\# Common Patterns Using AMPL

(Examples, Not Requirements)



AMPL is intentionally permissive and flexible.

The following examples illustrate common real-world ways developers separate

code, assets, and branding when using AMPL.



These examples are illustrative only. They describe patterns made possible by

AMPL but do not impose requirements or best practices.



---



\## 1. Games



Games often combine reusable code with creative assets such as artwork, music,

writing, and branding.



\### Example A: Game Code Under AMPL, Assets Restricted (Most Common)



Scenario:

\- You want the game logic to be reusable

\- You want to keep art, music, and writing under your control



Typical structure:



/src/           → Game code (AMPL-1.0)

/assets/        → Art, music, sounds (separate license)

/LICENSE.txt    → AMPL-1.0

/ASSETS.txt     → Asset license notice



Explanation:

\- Others may reuse or modify the code

\- Assets may not be reused without permission

\- Attribution to the code author must be preserved



---



\### Example B: Game Code Under AMPL, Assets Commercial



Scenario:

\- You sell the game

\- You want ports or mods to reuse the engine

\- Assets remain part of the commercial product



Result:

\- Engine reuse is allowed

\- Asset reuse is not

\- Ports may be closed or open

\- Attribution persists quietly



---



\### Example C: Open Game, Protected Name



Scenario:

\- You allow forks

\- You want to prevent clones from using your game’s name



Example notice:



The game code is licensed under AMPL-1.0.

The game name and logo are not licensed and may not be used

to imply endorsement.



AMPL does not grant trademark rights.

This separation is normal and recommended.



---



\## 2. Libraries (Infrastructure Code)



Libraries are often embedded into larger systems and benefit from minimal

compliance overhead.



\### Example D: Library Under AMPL, Used in Closed Software



Scenario:

\- You publish a reusable library

\- A company embeds it in proprietary software



AMPL allows:

\- closed-source embedding

\- commercial distribution

\- no license inheritance

\- no source disclosure



Obligation:

\- preserve attribution in documentation or credits



---



\### Example E: Partial Contribution Back



Scenario:

\- A developer improves part of the library

\- Keeps other changes private

\- Submits a clean patch upstream



AMPL behavior:

\- contribution is voluntary

\- only submitted code is licensed to the project

\- private work remains private

\- contributor may sell their enhancements separately



---



\## 3. Commercial Tools \& Applications



AMPL is designed to be commercial-safe by default.



\### Example F: Commercial Tool Using AMPL Components



Scenario:

\- you ship a paid desktop or CLI tool

\- you use one or more AMPL-licensed components



Compliance:

\- include attribution in NOTICE.txt, About screen, or documentation



No other obligations apply.



---



\### Example G: Open Core + Paid Extensions



Scenario:

\- core functionality under AMPL

\- advanced features sold separately



Structure:



/core/          → AMPL-1.0

/extensions/    → proprietary or commercial license



Result:

\- core remains reusable

\- extensions are protected

\- attribution persists

\- no viral spillover



---



\### Example H: White-Label or OEM Distribution



Scenario:

\- your software is redistributed under another brand



AMPL requires:

\- attribution remains accessible

\- no implication of endorsement



AMPL does not require:

\- UI branding

\- marketing acknowledgment

\- splash screens



This makes AMPL suitable for OEM and enterprise use.



---



\## 4. Applications \& Office Suites



Large applications such as office suites, mail clients, editors, and productivity

tools often combine core engines, plugins, file formats, UI assets, and branding.



AMPL is designed to support this complexity without forcing a single licensing model.



---



\### Example I: Office Suite Code Under AMPL, Assets \& Branding Separate



Scenario:

\- you build an office suite (word processor, spreadsheet, mail client, etc.)

\- you want the code to be reusable

\- you want to retain control over branding, icons, and bundled content



Typical structure:



/core/            → application code (AMPL-1.0)

/ui-assets/       → icons, themes, artwork (separate license)

/templates/       → document templates (separate license)

/branding/        → name, logo, trademarks

/LICENSE.txt      → AMPL-1.0

/NOTICE.txt       → attribution



AMPL allows:

\- forks of the code

\- closed or open redistribution

\- commercial editions

\- ports to other platforms



Assets and branding remain protected unless explicitly licensed.



---



\### Example J: Core Application Under AMPL, Plugins Proprietary or Mixed



Scenario:

\- core office application under AMPL

\- advanced features delivered as plugins or extensions



Structure:



/core/            → AMPL-1.0

/plugins/basic/   → AMPL-1.0 or permissive

/plugins/pro/     → proprietary / commercial



Result:

\- core remains freely reusable

\- plugin authors choose their own licenses

\- no forced disclosure

\- no license inheritance



---



\### Example K: Commercial Office Application Using AMPL Libraries



Scenario:

\- you ship a closed-source office or mail application

\- you use AMPL-licensed libraries (e.g., UTF-8 handling, file parsing)



Compliance:

\- include attribution in About dialog, NOTICE.txt, or documentation



No requirements:

\- no source disclosure

\- no publishing of modifications

\- no adoption of AMPL for your entire codebase



---



\### Example L: Forks, Rebrands, and Long-Term Maintenance



Scenario:

\- an office suite is forked after original development slows or stops

\- new maintainers take over

\- original authors are no longer involved



AMPL behavior:

\- forking is allowed

\- closed or open continuation is allowed

\- attribution to original authors persists

\- no requirement to track down original maintainers



This is especially important for long-lived productivity software.



---



\### Example M: Document Formats and Interoperability



Scenario:

\- your office suite defines file formats or parsers

\- others want to reuse them for compatibility



AMPL allows:

\- reuse of parsers and format code

\- commercial interoperability tools

\- closed or open implementations



This supports ecosystems rather than locking them down.



---



\## 5. One-Sentence Summary



AMPL lets you share code without giving up your assets, your branding, your business

model, or your future options.



