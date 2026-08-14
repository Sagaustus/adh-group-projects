# Group chapter projects — African Digital Humanities

One worked notebook per group, turning a dataset into a publishable chapter draft.

Each notebook runs the analysis end to end and produces the numbers and the figure the
chapter needs. It does **not** decide what they mean: cells marked **YOUR DECISION** are
where your judgement enters, and they are the only part a reader will credit to you.

## Open in Colab — nothing to install, nothing to upload

Click a badge. The first cell downloads the data straight from
[`adh-dh-datasets`](https://github.com/Sagaustus/adh-dh-datasets), so there is no upload
step and no account needed.

| Group | Dataset | Working chapter title | Open |
|---|---|---|---|
| 1 | African films on Wikidata | *A Title, a Country, an Identifier: thin records and the labour geography of African cinema on Wikidata* | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Sagaustus/adh-group-projects/blob/main/group-01-african-films/analysis.ipynb) |
| 2 | African languages (Glottolog) | *No Code, No Corpus: ISO 639-3 as a precondition for computational existence* | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Sagaustus/adh-group-projects/blob/main/group-02-african-languages/analysis.ipynb) |

## Writing the chapter, and dividing the work

Two sections at the end of each notebook exist because the analysis is the easy half:

**The chapter template (Step 9).** The full structure of a DH chapter — introduction,
the standard and its critics, data, method, findings, discussion, limitations,
conclusion — with sentence frames to complete and a note under each section saying
which notebook step feeds it. A cell then prints draft sentences with *your* computed
numbers already in place, so you can see which figure belongs in which section. Rewrite
them in your own voice; they are placement practice, not prose.

**Division of labour (Step 10).** Seven roles mapped to chapter sections and to the
expertise each draws on, a dependency diagram showing what has to happen before what,
and a CRediT contribution statement to fill in. Note that **Coder A and Coder B must
work independently** — that is a requirement of the method, not a staffing convenience.
Without two independent coders there is no agreement figure, and the qualitative
section has no evidential standing.

## What each notebook contains

The seven steps of the assignment, plus the two things that turn a report into a chapter:

1. **Frame** — one descriptive and one analytical question, with the method each needs.
2. **Absence audit** — a missing variable, a missing population, a level of detail too coarse.
3. **Describe** — the central variable, with a deliberate choice between mean and median.
4. **Compare** — two groups that matter, in units a reader thinks in.
5. **Test** — a test *and* an effect size.
6. **Show** — one chart, sorted deliberately, captioned with what was filtered.
7. **Limits** — the sentences the data does not support.
8. **The qualitative half** — a coding scheme, applied by two coders, with an agreement figure.
9. **The counter-practice** — who is already fixing this. A critique without one reads as a complaint.

## A note on the code

The notebooks deliberately walk into two errors before correcting them, because both are
common enough to sink a submission:

- **A rate computed over a denominator too small to mean anything** — countries with two
  films scoring 100% completeness.
- **Perfect collinearity** — you cannot control for a country-level variable *and* include
  country fixed effects, because the first is an exact linear combination of the second.
  The fit will not converge, and the fix is to decide which question you are asking.

## Licence

Notebooks CC BY 4.0. The datasets keep their own licences — see each dataset's
`CODEBOOK.md` in the datasets repository.
