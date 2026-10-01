# Blue Lens Researcher Network

Interactive directory and expertise network for the **Reinventing the Blue Lens** marine and coastal research network: Prince of Songkla University (PSU), Kasetsart University (KU), Chulalongkorn University (CU) and international partners.

Developed for the Faculty of Environmental Management, PSU, and the Coastal Oceanography and Climate Change Research Center (COCC).

**Live site:** https://OWNER.github.io/blue-lens-network/

## Features
- Search researchers by name, expertise, institution or faculty. Small typos still match.
- Filter by research theme, expertise topic, institution, position, country and profile details.
- Card and table views, researcher profiles, and suggestions for researchers with related expertise.
- Scopus metrics (h-index, documents, citations) where a Scopus author profile was found.
- Research topics from publications, auto-classified from OpenAlex records (2018–2026) and shown separately from self-reported expertise.
- Interactive expertise network. Turn themes, topic sources and institutions on or off, set a minimum number of shared researchers per topic, and find a researcher or topic on the map.
- Overview charts and a profile-completeness summary.
- Light and dark themes. CSV export of the current selection.

## Data
- `data/researchers.json` holds the public dataset (89 members) that is also embedded in `index.html`.
- Source: Marine Researcher Network PSU–KU–CU 2025–2026 registration sheet, cleaned and translated to English.
- Scopus metrics were retrieved on 1–2 Oct 2026 from public Scopus author profiles.
- Publication topics are auto-generated from OpenAlex (CC0) and have not yet been confirmed by the researchers.
- Personal email addresses are removed from the public version. Only institutional addresses are shown.
- Names marked **Name pending** were romanized from Thai and still need checking.

To request a correction, open an issue or contact the network coordinators.

## Tech
A single static `index.html` with no build step. [d3](https://d3js.org) is loaded from cdnjs for the network view and fonts come from Google Fonts.
