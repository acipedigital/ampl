\# Decision Matrix: Game vs Application vs Library



This matrix helps developers quickly choose a licensing pattern that fits the

type of project they are building.



AMPL is permissive and flexible. These recommendations describe common patterns

but are not requirements.



---



\## Quick Comparison



| Question | Game | Application / Office Suite | Library |

|--------|------|----------------------------|---------|

| Is the primary value in the code logic? | Yes | Yes | Yes |

| Are there creative assets (art, music, templates)? | Yes | Often | Rare |

| Do you want to keep assets proprietary? | Common | Common | N/A |

| Is closed-source distribution expected? | Common | Very common | Very common |

| Will others embed this into their own products? | Sometimes | Sometimes | Yes |

| Do you expect long-term forks or maintenance? | Sometimes | Yes | Yes |

| Is commercial use expected? | Yes | Yes | Yes |



---



\## Recommended Patterns



\### Games

Recommended:

\- Code: AMPL-1.0

\- Assets: separate license

\- Branding: trademark/usage notice

\- Attribution: credits or NOTICE file



---



\### Applications / Office Suites

Recommended:

\- Core code: AMPL-1.0

\- UI assets, templates: separate license

\- Plugins/extensions: developer’s choice

\- Attribution: About dialog, NOTICE file, or documentation



---



\### Libraries

Recommended:

\- Library code: AMPL-1.0

\- Downstream projects may remain closed-source

\- Attribution via documentation or NOTICE file



---



\## Rule of Thumb



If you want your code to travel freely, but your assets, branding, or business

model to remain yours, AMPL is a good fit.



