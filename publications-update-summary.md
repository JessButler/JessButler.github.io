# Publications page update: summary

## Context and goal

Workspace: `C:\Users\computer\Documents\JessButler.github.io`, a Quarto website for Jessica E. Butler (Lead Data Scientist at NHS Grampian and Senior Research Fellow at the University of Aberdeen). Key files are `index.qmd`, `publications.qmd`, `research.qmd` and `talks.qmd`, plus posts under `posts/`. ORCID: 0000-0003-2054-3777. Google Scholar: https://scholar.google.com/citations?user=N3iK7TcAAAAJ

Request: find publications by this author that were missing from the site's publications page, search the web thoroughly, find DOIs, search for conference abstracts, and update `publications.qmd`. Each entry should have a source link and DOI, and each conference abstract should be listed once alongside its full paper.

## Work done

1. **Original page.** `publications.qmd` held only five items, all from 2021-2022: the CYP mental health briefing, the BMC Psychiatry 2023 paper, the CEV briefing, the medRxiv shielding preprint, and two Health Foundation blog posts.
2. **Source gathering.** I compared the Scholar profile, ORCID (24 works, nothing after 2023), Crossref, PMC, Health Foundation pages and the Aberdeen research portal.
   - The Health Foundation site and the Aberdeen portal returned HTTP 403 on direct fetches.
   - Crossref intermittently returned HTTP 429.
   - Europe PMC returned nothing for her ORCID.
   - Of the 38 pages of the ACHDS publications list, I checked only pages 1-7, and found only the Scheliga 2026 entry.
3. **Rewrite.** I wrote a new `publications.qmd` with these sections:
   - Networked Data Lab and linked data
   - Children's mental health
   - Coronavirus
   - Open science and reproducibility
   - Multimorbidity and cohort studies
   - Mental health services
   - Earlier work in microbial genomics
4. **Layout.** Each entry has an author/year/title link, journal, and DOI where one exists. Conference abstracts and preprints are nested as sub-bullets under their full papers.
5. **Confirmed DOIs.**
   - IJPDS 2026: 10.23889/ijpds.v11i5.3600 (Butler & Knight), v11i5.3736 (elective care) and v11i5.3680 (Scheliga). The Scheliga paper also has an Aberdeen repository DOI, 10.20392/CK8D-YC88.
   - Social Science & Medicine 2024: 10.1016/j.socscimed.2024.117057. Its SSM abstract is 10.1136/jech-2024-ssmabstracts.2, and its preprint is 10.1101/2023.10.13.23296488.
   - Health Foundation: 10.37829/HF-2024-NDL01 (intermediate care), 10.37829/hf-2022-ndl1 (CYP briefing) and 10.37829/HF-2021-NDL01 (CEV briefing).
   - IJPDS 7(3) abstracts: 1897 (shielding), 1909 (provenance), 1912 (public involvement), and 1980 (children's mental health).
   - Lancet Infect Dis RECOVERY sotrovimab: 10.1016/S1473-3099(25)00361-5.
   - Journal of Neuroscience Methods UKRN paper: 10.1016/j.jneumeth.2023.109949.
   - The remaining DOIs came from her ORCID record.
6. **Better Homes briefing.** I confirmed from the Health Foundation page that "Jessica E Butler" is a listed author of *Better homes, better health: insights from linking housing and health data* (May 2026). I added it to the Networked Data Lab section as "Butler JE, et al. (2026)". The page showed no full author list and I found no DOI.
7. **2025 provenance paper.** I checked *Semi-automated data provenance tracking...* (IJPDS 10(2), DOI 10.23889/ijpds.v10i2.2464) in Crossref. The authors are O'Sullivan, Markovic, Dymiter, Scheliga, Odo and Wilde. Butler is not an author, so I left it out.

## Open items and caveats

- **No DOI found:** the 2025 Health Foundation elective care briefing, the Better Homes briefing, and the Ball et al. 2025 OP21 abstract (J Epidemiol Community Health 79 Suppl 1, A10-A11). Crossref was rate-limited when I tried the OP21 abstract. The two Health Foundation blog posts have no DOI.
- **Inferred and unverified:** the 1980 abstract DOI is inferred from its article number, and the ijpds.org source links for 1909 and 1980 follow the site's URL pattern without being opened. The 2022 IJPDS items are labelled "IPDLN conference abstracts" based on volume and numbering, not the conference programme. The author lists of several entries are truncated with "et al." from Scholar.
- **Deliberately left out:**
  - The Mahadevan 2006 and Geobacter review papers.
  - Hurricane sediment papers, the 1986 Fermilab report, and duplicate Scholar entries.
  - The 2016 Wood et al. poster, which is peer-reviewed but has no DOI.
  - The ICIC25 integrated care abstract from Prendergast (International Journal of Integrated Care, DOI 10.5334/ijic.ICIC25388), because I haven't confirmed Butler is an author.
- **Not yet done:** I haven't rendered the Quarto site to check the page displays correctly. `publications.qmd` is the only file changed.

## Possible next steps

- Render the site and check how `publications.qmd` displays.
- Add the full author list and a DOI for the Better Homes briefing if you can supply them.
- Retry the Crossref lookup for the Ball et al. 2025 OP21 abstract DOI.
