# HMC hearing — experimental design audit, 2026-09-08

Audits the nine studies the Human–Machine Communication hearing (`manuscript/PAPER.md`, lines 59–90)
cites as empirical support, against the existing literature cards (`cards/`) and, where the cards
lacked hard methodological detail, the primary sources themselves. Every number below was read from a
fetched source this round, not reconstructed from memory or from the card's prose — sources are named
per item. Two sources (Hohenstein & Jung 2020; Hohenstein et al. 2021/2023) were fetched to full text;
three (Sundar & Nass 2000, Sundar & Kim 2019, Jung/Martelaro/Hinds 2015) were blocked by publisher
paywalls (SAGE, ACM DL) on every route tried and remain at the cards' existing depth.

---

## 1. Per-study methods notes

### Nass & Moon (2000) — CASA programme summary
Review article, not a single experiment; no new data. The card's account (mindlessness explanation,
CASA's decade of findings) is accurate and sufficient. No fetch needed.

### Sundar & Nass (2000) — source orientation
**Not independently verified this round — blocked.** SAGE returned HTTP 403 on both the DOI redirect
and the direct journals.sagepub.com URL; academia.edu and ResearchGate mirrors are not fetchable
without login. Web search confirms the design shape without numbers: two studies, both manipulating
who the participant is told authored identical computer output (Study 1: computer vs. the programmer
behind it; Study 2: a constructive replication substituting a "networker" for the programmer), and
both find source attribution changes evaluation of identical content — consistent with the card. No N,
no F/p values, no effect size could be confirmed from any accessible source. **This is the paper's
single most load-bearing citation** (line 65: "the experimental ground for the first operation") and
currently carries zero verified quantitative detail anywhere in the project's literature apparatus —
the card itself already flags this ("cite for the construct, not for effect sizes"), so the gap is
long-standing, not new. See §5.

### Sundar & Kim (2019) — machine heuristic
**Not independently verified this round — blocked.** ACM DL returned 403 on both the DOI redirect and
the fullHtml mirror; a third-party PDF mirror (library.usc.edu.ph) refused the connection. Web search
(unverified against the primary text) surfaces a plausible N=160 and an airline-reservation
credit-card-disclosure task, with disclosure difference concentrated among participants who already
scored high on machine-heuristic endorsement — but this figure comes from a search-engine summary, not
a direct read, and should not be cited without confirmation. See §5.

### Hohenstein & Jung (2020) — "moral crumple zone"
**Verified in full** via `hohenstein.infosci.cornell.edu/files/AI_crumpleZone.pdf` (author-hosted,
open).
- **Sample:** N = 113 (75.2% female), on-campus recruiting system at a large northeastern-U.S.
  university, ages 18–25 (M = 19.28, SD = 1.21), course credit.
- **Design:** 2 (successful vs. unsuccessful conversation, controlled by a confederate running a
  scripted script) × 2 (standard messaging app [WhatsApp] vs. AI-mediated [Google Allo with smart
  replies]), between-subjects. Cells: successful/standard N=25, successful/AI-mediated N=25,
  unsuccessful/standard N=24, unsuccessful/AI-mediated N=24.
- **DVs:** self-reported percentage-allocation of responsibility for the outcome (self / partner /,
  in AI conditions, the AI); a 5-item trust scale (α = 0.92) rated separately for partner and AI.
- **Key results, unsuccessful conversations:** partner responsibility, standard M=83.5 (SD=21.96) vs.
  AI-mediated M=64.04 (SD=32.57), F=5.89, p=.019, η²=0.11. Partner trust, standard M=1.92 vs.
  AI-mediated M=3.04, F=6.19, p=.017, η²=0.12. AI itself received significant nonzero attribution only
  in unsuccessful conversations (bootstrap 20%-trimmed mean 7.5, 95% BCa CI [1.38, 18.13]; successful
  conversations' CI included zero: [0.0, 4.93]).
- **Limitation the card didn't state explicitly:** the "partner" was a confederate secretly controlling
  the outcome, so what changed was the participant's *attribution*, not any real behavior difference by
  a human partner — the effect is squarely about perception, which is exactly the register the paper's
  claim needs, but the paper should not imply a real second human's behavior changed.

### Hohenstein et al. (2021 preprint / 2023 *Scientific Reports*) — smart replies at scale
**Verified in substantial part** via arXiv:2102.05756v1 (Feb 2021 preprint; the published *Scientific
Reports* 13:5487 version was blocked by Nature's login gate on every route). Treat figures below as
preprint-sourced and re-check against the published VoR if exact numbers are quoted in text.
- **Two experiments, n = 1036 total**, matching the published abstract's headline figure.
- **Experiment 1** (the cooperation/affiliation study): N=438 individuals (219 pairs), Mechanical Turk,
  33.7% female, ages 18–68 (M=34.15, SD=10.1), paid. Randomly assigned to three smart-reply conditions
  (both partners can use SR / one partner only / neither), discussing a real MTurk grievance topic.
  Instrumental-variable estimation (not a simple ANOVA) isolates the causal effect of *actual* SR use
  from confounds. Key results: self's SR use → more efficient communication, t(198)=2.21, p=.0286;
  perceived partner SR use correlated only weakly with actual use (Pearson's r=0.22, t(97)=3.62,
  p=.0005); perceived partner SR use predicted *lower* cooperativeness rating, t(92)=−9.89, p<.0001,
  and lower affiliation, t(92)=−6.90, p<.0001 — even controlling for the partner's actual use. But
  actual partner SR use, via IV estimation, predicted *higher* cooperation, t(167)=2.23, p=.0273, and
  *higher* affiliation, t(167)=2.54, p=.012.
- **This is the precise shape of the "suspicion" finding, and it is more specific than the current
  PAPER.md prose.** The penalty attaches to *perceived* smart-reply use (a belief, weakly correlated
  with reality), not to a manipulated "suspicion" condition — nobody in Experiment 1 was told or shown
  evidence their partner used AI; participants simply guessed, and the guess (right or wrong) predicted
  the penalty. "A participant suspected of using them was evaluated more negatively" (PAPER.md line 77)
  is a fair gloss but elides that the suspicion is unprompted and self-generated, not induced — a
  sharper, more defensible sentence is available: *perceived* smart-reply use, largely uncorrelated
  with actual use, predicted lower cooperation and affiliation ratings.
- **Experiment 2** (the sentiment study): N=598 individuals (299 pairs), between-subjects, four
  conditions (Google's real smart replies / positive-sentiment replies / negative-sentiment replies /
  no replies), policy-issue discussion, VADER sentiment scoring. Positive/Google-reply conversations
  scored more positive than negative/no-reply conversations, t(127)=2.75, p=.007, d=.352.
- **IRB and pre-registration:** IRB #1610006732; pre-registered on AsPredicted (#40389) — worth noting
  since the paper's own empirical section currently lacks a stated stopping rule (2 Sept panel item 12,
  row 221) and this is a clean comparator the author could cite for what a pre-registered smart-reply
  design looks like.

### Jung, Martelaro & Hinds (2015) — robot conflict repair
**Not independently verified this round — blocked.** ACM DL 403'd; no alternate open copy located in
the time available. The card's account (robot intervenes with conflict-repair utterances between two
human partners; the intervention shifted interpersonal perceptions; framing of the intervention
moderated the effect) is consistent with the paper's characterization and the two Crossref-record
caution (full paper vs. late-breaking abstract) is already correctly resolved in the card. No N or
stats confirmed. See §5.

### Traeger et al. (2020) — vulnerable robots (PNAS)
Not re-fetched this round; the existing card already carries the hard number the paper uses (51
groups of three humans and one robot) and PNAS is open access, so this card's "full_text" depth is
credible without a re-check. No discrepancy found against PAPER.md line 83.

### Seeber et al. (2020) and Sebo et al. (2020) — agenda paper and systematic review
Neither carries primary data; both cards are argument-summaries of programmatic/review pieces, which is
the right depth for how PAPER.md uses them (as scope-of-the-field evidence, not as effect claims). No
gap.

### Suchman (2007) and Gibbs et al. (2021) — theoretical, out of scope per the task's own framing (not
experimental). Cards read fine against PAPER.md's use of them.

---

## 2. Accuracy check against current PAPER.md prose (lines 59–90)

- **Line 65** ("Sundar and Nass... found the results largely held"): the phrase "largely held" belongs
  to Reeves & Nass 1996 replication generally, not specifically to the Sundar & Nass 2000 source-
  orientation manipulation, which is a two-study design testing attribution, not a replication check.
  Minor imprecision; worth a look but not urgent given the sentence's overall claim is correct.
- **Line 77** ("a participant suspected of using them was evaluated more negatively") — see the
  Hohenstein et al. note above. Accurate in substance, imprecise on mechanism (perceived, not induced,
  suspicion). A one-clause fix ("perceived, often mistaken, smart-reply use...") would tighten this
  without adding length.
- **Line 77** ("borrowing Elish's (2019) term, they call the machine a *moral crumple zone*") —
  confirmed correct against both the Elish card and the fetched Hohenstein & Jung 2020 full text
  (they cite Elish 2016/2019 explicitly in their §2.2).
- **Line 83** ("Traeger et al. (2020) ran fifty-one groups of three people and one robot") — confirmed
  correct against the existing card; no fetch needed to re-verify.
- No other factual errors found in lines 59–90 against what could be verified this round. The three
  blocked sources (Sundar & Nass 2000, Sundar & Kim 2019, Jung et al. 2015) are used for framing claims
  in PAPER.md that the cards already support at the right depth — nothing in the current text overreaches
  into unverified statistical territory for those three, which is itself informative (the authorial
  discipline the cards' "cite for the construct, not effect sizes" instruction produced is visible in
  the prose: PAPER.md never quotes a number from any of the three blocked sources).

## 3. What's new since original publication

- **Zhu & Molnar (2026), "Blissful (A)Ignorance: Despite the widespread adoption of AI in communication,
  people do not suspect AI use in realistic contexts,"** *Computers in Human Behavior* (same journal as
  Hohenstein & Jung 2020), published mid-2026 — after every other source in this hearing. Two online
  experiments, >1,300 U.S. adults, realistic communication contexts (email, social media, texting).
  Finding: in naturalistic settings, people default to treating messages of unknown origin as
  human-written and rarely suspect AI involvement, even as self-reported personal AI use rises — the
  "blissful ignorance" does not erode over time. It *confirms* the penalty when suspicion is triggered
  (disclosed or strongly suspected AI use lowers trust/authenticity ratings, consistent with Hohenstein
  et al.) but supplies the missing base-rate: the mechanism this hearing leans on fires rarely outside
  the lab. **This is a genuine, citable complication of line 77's claim** and the single strongest
  candidate for a new citation in this hearing — it does not overturn the moral-crumple-zone or
  suspicion-penalty findings, it bounds their real-world frequency, which is exactly the kind of
  qualification a hostile reviewer would otherwise supply for the author.
- Two more recent, adjacent hits surfaced by search but not read in full (flagged, not verified):
  "Who wrote this? How smart replies impact language and agency in the workplace" (ScienceDirect,
  S2772503023000221) — a workplace-context extension, which would be directly on-point for a paper
  about coordination at work if verified. "Explaining the Reputational Risks of AI-Mediated
  Communication" (arXiv:2509.09645) — a 2026 working paper on how AI-labeled messages are read as less
  diagnostic of moral character. Neither is verified enough to cite; both are candidates for the
  author to pull and read before Lima if the HMC hearing is being actively developed rather than only
  trimmed.
- No newer work located that changes how the paper should characterize Sundar & Nass 2000's source
  orientation or Jung et al. 2015's robot-mediated repair; searches for replications of both came back
  empty in the time available.

## 4. Length-justification verdict

**The hearing's length is earned, not padded, on the evidence gathered this round — more so than the
8 Sept structure review's raw proportion count suggested.** Every sentence checked traces to a distinct
study and a distinct, non-redundant claim: source orientation (Sundar & Nass), the machine heuristic
(Sundar & Kim), the crumple-zone attribution shift (Hohenstein & Jung), the suspicion/perception penalty
at scale (Hohenstein et al.), robot-mediated repair (Jung et al.), vulnerable-disclosure improving
human-to-human coordination (Traeger et al.), the teaming agenda (Seeber et al.), the systematic-review
gap (Sebo et al.), and the asymmetric-interpretation diagnosis (Suchman). Four generations, four
distinct empirical traditions (CASA lab experiments, AI-MC field-scale experiments, HRI group studies,
STS theory) converging on one boundary claim. That is a lot of ground to cover in four subsections and
roughly 1,850 words, and this round did not find a sentence that only restates a claim another sentence
in the same hearing already made — the repetition the 8 Sept panel found (lines 61/89's trajectory
recap) is real but is the *only* clean duplication in the hearing, and it's already in the approved cut
list.

Where there is room, on this evidence, is not inside the hearing's citations but in the *connective and
self-narrating* prose around them — exactly what both panels' Band 1 already targets (line 67's second
sentence, line 79's "which the demarcation has to accommodate rather than deny," the roboticist sentence
that could open its paragraph instead of arriving mid-stream). The findings themselves do not compress
further without losing a distinct, verifiable claim. If the paper needs the HMC hearing shorter than
its post-Band-1 length, the honest move is not prose compression but dropping an entire study's
paragraph (most likely Seeber et al., the only one of the nine that is agenda-setting rather than
data-bearing, and already substantially covered in argument by Sebo et al.'s review) — not tightening
sentences that are each the only place a specific finding's nuance lives.

## 5. Papers to source

The author should pull these directly (institutional access will clear the 403s this round hit):

1. **Sundar, S. S., & Nass, C. (2000). Source orientation in human-computer interaction.**
   *Communication Research*, 27(6), 683–703. SAGE. **Highest priority** — this is the hearing's single
   most load-bearing citation (line 65) and the project's literature apparatus has never held a
   verified N, condition detail beyond the card's paraphrase, or a single statistic from it. A
   university library SAGE Journals login should retrieve it directly.
2. **Sundar, S. S., & Kim, J. (2019). Machine heuristic.** CHI 2019. ACM DL. Needed to confirm or
   correct the unverified N=160 figure found via search, and to get the mediation statistics referenced
   in the card's "relation to the argument" section.
3. **Jung, M. F., Martelaro, N., & Hinds, P. J. (2015). Using robots to moderate team conflict.**
   ACM/IEEE HRI 2015. ACM DL. Lower priority than the two above — the paper's use of this study is
   already appropriately light (one sentence, no statistics claimed) — but worth a read if the author
   wants to strengthen rather than merely preserve this citation.
4. If the exact published-version numbers matter for a direct quote, **re-confirm Hohenstein et al.'s
   figures against the *Scientific Reports* 13:5487 version of record**, not the 2021 arXiv preprint
   used here — Nature's access gate blocked every route tried this round, but the two should not differ
   materially given the abstract's n=1036 matches on both versions.
