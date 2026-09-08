# Methodology Review — PAPER.md (post-cut)

**Manuscript:** "Algorithmacy: A Competency for Coordinative Co-optation" (Dissertation Paper 2; OS/OT PDW, Lima, October 2026)
**Version reviewed:** `manuscript/PAPER.md` as cut on 2026-09-01 — body 10,219 words (from 18,079); Empirical Strategy 692 words in two subsections; Appendices A–C untouched at 3,758 words
**Review date:** 2026-09-02
**Lens:** research design; insider action research (Coghlan & Brannick); abduction (Timmermans & Tavory); construct development and psychometrics (Suddaby; formative vs. reflective; nomological networks; discriminant validity); critical incident technique (Flanagan); sampling and power; falsification criteria; IRB and ethics disclosure
**Scope:** content only. Line numbers are `grep -n` positions in PAPER.md. Body is lines 13–228; Appendix B is 450–538; Appendix C is 540–575.

---

## Verdict

**Minor-to-moderate revisions, with one structural repair.** The cut did what a cut should: the site's three gate properties, the pilot count, the researcher-blind procedure, the IRB status, and the power concession all survived into the body intact, and every Study 2/3 pointer in the body lands on a real paragraph in Appendix C. The predecessor's two heaviest findings — the missing scale-development step and the confirmation-shaped stopping rule — are fixed in Appendix C exactly as prescribed.

What the paper still lacks is a stated measurement model. Line 175 says the three operations are neither reflective indicators nor formative components; line 225 asks whether they load onto a higher-order factor; Study 2 fits a confirmatory model with per-operation latent correlations. Those three statements describe three different models, and no sentence in body or appendix says which one the CFA will estimate. The same gap runs downstream: the Paper 3 panel is described as tracking within-person trajectories and running a wave-2 convergence check, but the algorithmacy items that would make either possible are not built until Study 2. Fix the measurement model and the panel's contents, and the empirical section becomes as disciplined as the construct section already is.

One body ↔ appendix inconsistency the cut introduced: the body's RQ4 paragraph (line 219) now gives only the attribution-versus-*keeping track* rationale, while the construct section (171) and Appendix B (456) make *interpreting* the null host and the primary comparison. That is the exact wavering four reviewers flagged last round, reintroduced by deleting one sentence.

---

## Step 0 — Register

A formal construct-development paper in the *Organization Theory* idiom, Suddaby-organized, with an insider-action-research methods appendix in the Coghlan–Brannick vocabulary. I hold the design to the standards it cites for itself — Pratt (2009) on method-puzzle alignment, Timmermans and Tavory (2012) on abductive surprise, Zhou et al. (2025) as the psychometric benchmark the paper names as its own — and I read the body as a PDW discussant would: first, alone, and only then with the appendices open.

---

## Part 1 — Design and measurement

### Finding 1 (Major). The three-wave panel has no algorithmacy instrument, and the body does not notice.

**Where.** Body line 221: the panel "tracks within-person trajectories and is not powered for factor analysis, which Study 2 takes up." Appendix B line 517: the survey serves "tracking within-person developmental trajectories across the semester, and administering Zhou et al.'s (2025) scale at wave 2 as a descriptive convergence check with *interpreting* and *specifying intent*." Appendix C line 552: "Study 2 begins by building the instrument the confirmatory model requires. I convert the Study 1 incident corpus into a candidate item pool."

**Why it matters.** The items that measure *interpreting* and *specifying intent* are generated from the Study 1 corpus, after Study 1 closes. So at wave 2 of Study 1 there is nothing for Zhou's *Understanding* and *Leveraging* subscales to converge with, and the "developmental trajectories" the panel tracks are trajectories of an unnamed quantity. The predecessor raised the convergence-check problem (§1.2, item 1); the author fixed Study 2 and left the panel untouched, which sharpened the gap rather than closing it.

**Fix.** State the panel's contents. Two defensible answers exist, and the author may want both. (a) Provisional items: a short pool written from the four pilot modules and the construct definitions, administered as a development pilot whose item statistics feed Study 2's generation step — say so, and stop calling the wave-2 comparison a convergence check. (b) Behavioral indicators the site already computes: the gate prices each reviewer's accuracy (line 215), and the repository records resubmission counts, pull-request description revisions, and time-to-clear. Those are non-self-report proxies for the three operations, and they exist because the author built the gate. Naming them makes the panel the one arm of the design no gig-platform study could run.

### Finding 2 (Major). The nomological network states four predictions and Study 2 operationalizes one.

**Where.** Body line 159 embeds algorithmacy against four neighbors "and state[s] each relation as a testable prediction, pre-registered for the pooled sample in Study 2 (Appendix C)." Appendix C lines 556–562 pre-register three Zhou pairings (*Understanding*–*interpreting*, *Leveraging*–*specifying intent*, *Embracing*–null) and an HTMT threshold. Nothing in Appendix C names an instrument for Rahman's reactivity, Spitzberg's CMC competence, or Sutherland's gig literacies.

**Why it matters.** Rahman (2021) built a qualitative typology, not a scale; Sutherland et al. (2020) built a fivefold typology from 39 interviews, not a scale with a *relationship-building* subdimension one could correlate against. The body's predictions about both therefore have no test anywhere in the agenda. Spitzberg (2006) does have a self-report CMC competence measure, and it does not appear in Study 2. Three further problems sit inside the one prediction that is operationalized. "Pre-registered" is written as an accomplished status with no registry, date, or link; the author has registered nothing, because the instrument does not exist. The predicted null with *Embracing* — the paper's own "sharpest single test" — has no equivalence bound; at N = 200–250 a non-significant *r* is not a null result, and a reader who knows the psychometric literature will ask for a smallest effect size of interest and a TOST.

**Fix.** In the body, claim only what Study 2 tests: "Study 2 operationalizes the algorithmic-competency and machine-heuristic relations; the reactivity and gig-literacy predictions await instruments those literatures have not built, and I state them as directional expectations for Study 4's commercial sites." Add Spitzberg's measure to Study 2. Replace "pre-registered" with "to be pre-registered before Study 2 fielding." Set an equivalence bound for the *Embracing* null (|*r*| < .10 is the conventional choice; whatever the author picks, print it).

### Finding 3 (Major). The measurement model is undetermined, and three passages describe three different ones.

**Where.** Body line 175: "The operations are therefore neither reflective indicators of a single latent trait nor formative components of a static index; the survey establishes that they are distinct from neighboring constructs, and the critical incident technique shows that they operate as the loop Figure 1 depicts." Body line 225: "Whether the three operations load onto a coherent higher-order factor, hold empirical independence, or separate cleanly … are open questions that psychometric testing must resolve." Appendix C lines 556–562: a CFA with per-dimension latent correlations against Zhou's subscales.

**Why it matters.** "Neither reflective nor formative" is not a measurement model; it is a refusal of both. A CFA that produces latent correlations for *interpreting* and *specifying intent* separately is, by construction, fitting three first-order reflective factors — each operation as a latent variable with its own items. Whether a second-order factor sits above them is an empirical comparison (correlated-factors model vs. second-order model), which is what line 225 asks and line 175 seems to forbid. The pre-cut paragraph (archive line 286) said the operations are "psychometrically separable for discriminant testing" while the loop is a process claim tested qualitatively; compression turned that division of labor into a contradiction.

The process claim has its own problem. "The critical incident technique shows that they operate as the loop" is stated as though it were a result, and no disconfirming criterion for the loop exists anywhere — Table B1 is per-operation. What would falsify recursion? Incidents in which *specifying intent* precedes any interpreting; incidents in which a detected rule shift produces no change in the next interpretation; operations that appear in isolation across a participant's whole incident set. Flanagan's technique can carry that test — each module already elicits "baseline objective, system determination, tactical adaptation, resolution" (line 503), which is an ordered sequence — but only if the coding rubric records order and the paper says what proportion of unordered or one-operation episodes would kill the loop.

**Fix.** Replace the line-175 sentence with the model: three first-order reflective factors, one per operation, correlated; the higher-order structure is left open and Study 2 compares the two models. Keep the loop as a process claim and give it a row in Table B1: "Episodes coded for operation sequence; the recursive model is disconfirmed if a majority of complete episodes show *specifying intent* without prior *interpreting*, or *keeping track* without a subsequent change in interpretation." Delete "the survey establishes" for the Paper 3 panel, which the paper elsewhere says cannot establish it.

### Finding 4 (Major). Who retunes the weights? Adaptivity, the no-intervention pledge, and the Study 2 freeze are in three-way tension.

**Where.** Body line 213: "I will execute no further interventions within the focal cohorts." Body line 215 and Appendix B line 488: "weights and thresholds are retuned over the term." Appendix B line 492: "the gate operates autonomously, without instructor voting or manual grading overrides." Appendix C line 554: pooling requires "freezing the gate configuration across all pooled cohorts" or invariance testing.

**Why it matters.** The rule moves — that is a confirmed fact and the site's warrant for adaptivity. Something moves it. If the author, as course designer, retunes weights mid-term, that is an intervention in the focal cohort's gate mechanism, and the Coghlan–Brannick thesis-project pledge at line 213 is violated in the one place it most matters. If a schedule fixed before the term retunes them, the pledge holds, but the paper must say so. Either way, the true aggregation rule is known to the designer at every point in the term, which is the ground-truth asset the predecessor asked the author to claim (R6) and which remains unclaimed: participants' interpretings can be scored for *accuracy* against the actual rule, an evaluative criterion Rahman, Zhou, and Sutherland could never have had because their platforms were opaque to the researcher too.

The Study 2 freeze compounds it. "Freezing the gate configuration across all pooled cohorts" as written removes the retuning, and with it the adaptivity the construct's scope conditions require (line 155). What can be frozen without dissolving the form is the *retuning schedule* — the same sequence of weight changes at the same weeks in every pooled cohort — so that each cohort faces an identical moving rule.

**Fix.** One disclosure paragraph in Appendix B ("Research Site Architecture"): who or what retunes, on what schedule, fixed when, and known to whom. Then reword line 554: "freezing the retuning schedule — not the rule — across pooled cohorts." Then claim the asset: "Because I hold the true rule, RQ1's interpretings are scored for accuracy against it, not only coded for content."

### Finding 5 (Moderate–Major). Table B1's disconfirming criteria cannot tell construct failure from gate misspecification.

**Where.** Table B1 rows 1–2 and 4 (lines 533–536); body line 173 on the pilot incident; Appendix C line 548 on the fourth operation.

**Why it matters.** Row 1 disconfirms *interpreting* if participants "reconstruct evaluative outcomes exclusively from source code syntax and technical compiler logs without referencing peer evaluators." Row 2 disconfirms *specifying intent* if participants "achieve consistent evaluative success through isolated technical optimization without adopting dual-audience encoding." Both patterns would also result from a gate whose peer component carries negligible weight. If the machine-only router in the pilot cleared the gate, that tells us either that peers rated machine-optimized prose well (so dual-audience encoding is not a distinct demand) or that the peer weight is too small to price her illegibility (so the site does not instantiate mutual bindingness at the strength the construct needs). The first falsifies the construct; the second falsifies the site. Table B1 does not distinguish them, and the author is the one person who can — he knows the weights (Finding 4). Two smaller problems: row 2 requires "consistent" success, which one incident cannot show, and the body (173) never says whether the pilot participant's pull request actually passed; and row 4's criterion (appeals routed only to administrators) tests whether attribution is triadic at all, not whether it separates from *interpreting*, which is the question RQ4 asks. The separation test lives only in Appendix C line 548, as a one-directional dissociation ("decode successfully yet cannot discern" the source) with no counter-case and no threshold for "systematically."

**Fix.** Add a column or a footnote to Table B1: "Construct disconfirmation requires the pattern to hold where the peer component's weight exceeds [the stated threshold]; below it the pattern indicts the gate." State whether the pilot submission passed. Rewrite row 4's criterion as the dissociation and give it a count: "Attribution is a fourth operation if at least *k* participants show accurate decoding with failed attribution, or the reverse, across independent incidents."

### Finding 6 (Moderate). The body's RQ4 paragraph regressed to the tracking-only rationale.

**Where.** Body line 219: "does resolving the locus of authority function as an independent fourth operation? An actor may detect that a standard has moved without diagnosing the locus of failure for a single outcome, and the measurement model leaves that separation open." Body line 171: "I house attribution provisionally within *interpreting*, and that placement is the null hypothesis the measurement model carries." Appendix B line 456: attribution "separates from that operation [*interpreting*] and, secondarily, from longitudinal tracking." Table B1 row 4: "separate causal attribution from interpreting and from longitudinal rule tracking."

**Why it matters.** The pre-cut text (archive line 371) said "RQ4 tests whether evaluative attribution, provisionally housed within *interpreting*, separates empirically from both *interpreting* and *keeping track*," then gave the tracking rationale. The cut kept the rationale and dropped the sentence that named the primary comparison. A reader of the body alone now sees RQ4 justified against *keeping track* and the null housed in *interpreting* fifty lines earlier, with nothing joining them. Appendices are consistent; the body is not.

**Fix.** Restore one sentence at line 219 before "An actor may detect": "RQ4 tests whether attribution — housed provisionally within *interpreting* — separates from that operation and, secondarily, from *keeping track*."

### Finding 7 (Moderate). Appendix B claims evidence from the developmental cohorts that the design says do not exist as data.

**Where.** Appendix B line 468: "demographic shifts isolated behavioral variance from confounding human-capital baselines." Line 482: "the construct's operations were elicited under three different concealment regimes rather than one, so the behaviors recorded do not depend on any single interface." Line 480: in Trinidad, "automated operational logs were not retained." Line 484: the preliminary cohorts "are the developmental foundation rather than the formal empirical corpus." Body line 221: two pilot transcripts, one read informally.

**Why it matters.** "Elicited," "recorded," "isolated behavioral variance" are evidentiary verbs. The corpus behind them is one informally read transcript, from an unnamed cohort, plus unretained logs. The author fixed the predecessor's "intrinsic" overclaim by narrowing the claim, but the narrowed claim still asserts observation across three regimes that nothing in the paper documents. This collides with the core/thesis split the paper otherwise deploys correctly: if the developmental cohorts are not data, the paper cannot cite them as showing anything. A related misattachment: the strategic-research-site warrant (Merton, 1987; Eisenhardt & Graebner, 2007; lines 472–474) is argued for the *Trinidad* cohorts — no prior platform conditioning, simultaneous first encounter — and those cohorts yield no Paper 3 data. The Hult cohort's own warrant is the "hard case for opacity" at line 490, which the body no longer mentions.

**Fix.** Recast lines 468 and 482 as design history: "Across the cohorts I varied the concealment regime three ways; the formal protocol is therefore not tuned to any single interface." Move the strategic-site argument to Hult or delete it; if kept, say what makes business-school students at Hult a revelatory site for a phenomenon Rahman studied in freelancers. Put one sentence of the hard-case framing back in the body.

### Finding 8 (Moderate). The exit-rights caveat was reframed from a structural gap to a documentation gap, and the stakes gradient is still unaddressed.

**Where.** Body line 215: "One parameter remains undocumented … what exit and escalation rights a contested verdict carries. Until the contestation pathway is catalogued, the site's correspondence to the form on that dimension is unestablished." Pre-cut archive line 361 added: "A student's option to drop a course is not the analogue of unilateral account termination." Body line 33 and Table A1 line 437 define the form partly by the platform's power to "unilaterally terminate accounts."

**Why it matters.** Cataloguing will not change what a course gate can do. It can fail a submission; it cannot revoke enrollment, and the sanction that defines the form on the Stark–Pais account is not in the site's repertoire. The deleted sentence said that; the surviving one implies the gap closes once the paperwork is done. This is the same bindingness-intensity point the predecessor raised (§1.2): the site is a hard case for opacity and an easy case for stakes. Rahman's constrained reactivity — withdrawal to protect reputational capital — is a behavior that may not appear at all when the downside is a resubmission. Nothing in body or appendix concedes it.

**Fix.** Restore the deleted sentence. Add one more: "Stakes at the site are grade-level, not livelihood-level; behaviors that Rahman (2021) ties to dependence may not surface here, and Study 4's commercial sites are where the stakes gradient is tested."

### Finding 9 (Moderate). The body states the site and the status and none of the analytic logic.

**Where.** Body lines 213–221. Timmermans and Tavory, Flanagan, Blumer/Bowen, Gioia, and the pre-specified negative case (Appendix B line 511) appear zero times between lines 13 and 228. Line 213 promises "the falsification criteria summarized here"; the body summarizes one (the *specifying intent* pattern) and one exclusion (merge drift).

**Why it matters.** A discussant reading the body learns what the instruments are and when they field, but not how the transcripts will be analyzed, what stops the analysis, or what would falsify the tripartite model as a whole. The cut plan promised to reduce the strategic-site/abductive paragraph "to a parenthetical citation"; the executed cut removed it entirely. The negative case — a participant who resolves breakdowns through technical mastery alone, without conceptualizing the peer — is the paper's single best falsifier and lives only in an appendix.

**Fix.** Two sentences at the end of line 221: one naming the abductive logic and its stopping rule (incidents cased against the three operations and against skill acquisition, gig literacy, and dyadic sensemaking; analysis stops only when new incidents neither exceed the operations nor fit a rival better), one naming the negative case (a participant who clears the gate through technical mastery alone, never conceptualizing the peer, falsifies the triad's necessity).

### Finding 10 (Minor–Moderate). Ethics and procedure disclosures are thinner than the IRB line suggests.

**Where.** Body line 221 and Appendix B line 517 (IRB exempt, Protocol 260511078); Appendix B lines 492, 503, 515. The word "consent" appears nowhere in the manuscript. Line 503 ends with the participant validating "the final transcript for transmission" — to where, held by whom, is unstated. Whether the in-editor protocol is opt-in, and therefore self-selected, is unstated.

**Why it matters.** An exempt determination does not remove the need to say how consent is obtained from students whose instructor is the researcher, or where AI-generated interview transcripts go. Self-selection into the qualitative arm is a sampling question the design must own: if the students who complete the protocol are the ones who engaged most, the corpus over-samples the operations it is looking for. And the predecessor's interviewer-agent question (§1.5) is still open: an LLM interviewer probes differently across sessions, and nothing states the agent's prompt version is fixed, its outputs logged as part of the protocol, or its generative tendencies audited against the transcripts it produced.

**Fix.** Four sentences in Appendix B: consent mechanism; transcript destination and custody; whether the protocol is required or opt-in, and how selection is handled; the interviewer agent's fixed prompt version and logging.

### Finding 11 (Minor). Proposition 1 has no test, and the cohort-level falsifier has no sample.

**Where.** Body lines 193, 197–201; Appendix C lines 566–568, 572–574. Study 3 "tests Proposition 2 and the workforce-level aggregation mechanism"; Study 4 tests Proposition 3. Proposition 1 — individual gains with procedural justice unchanged — is assigned to no study, and its dependent variable (procedural justice, operationalized as "institutional disclosures won, formal appeals granted, or rules rendered legible to peers") is measured nowhere. Line 193's falsifier ("identical friction rates would falsify the claim") requires multiple cohorts under identical gates; Study 3's "sample and setting remain to be specified."

**Fix.** Assign Proposition 1 to Study 3 with appeals-granted and disclosures-won as its outcome measures; state that the cohort-level test needs at least two cohorts on the same retuning schedule, which the Study 2 pooling already supplies.

### Finding 12 (Minor). Two Table B1 wordings do not match the body's use of them.

Body line 215 says Table B1 "states exactly" that merge-driven drift is excluded; row 3 (line 535) names "public announcements or compiler updates" and never mentions repository history. Row 1 (line 533) says the pilot "validated" incident capture; one informal read validates nothing. Reword row 3 to include "repository history"; reword row 1 to "elicited."

### Finding 13 (Minor). Study 2's sample arithmetic is unstated.

Line 552 fits the EFA "on the first pooled cohorts"; line 556 runs the CFA at 200–250. Zhou et al. used disjoint samples (EFA N = 275, CFA N = 213). If the author follows the benchmark, that is six to seven cohorts of roughly fifty; if EFA and CFA share a sample, say so and defend it. Either way, state the number of cohorts and terms Study 2 implies.

---

## Part 2 — Body ↔ appendix consistency after the cut

| Claim | Body (line) | Appendix (line) | Consistent? |
|---|---|---|---|
| Attribution housed provisionally in *interpreting*; that is the null | 171 | B 456; C 548 | Yes |
| RQ4 tests separation from *both* interpreting and keeping track | 219 — tracking rationale only | B 456, B1 row 4 (536) — both | **No.** Body lost the "both" sentence; see Finding 6 |
| Pilot count: two transcripts, first read informally, second unread | 221 | B 521 | Yes |
| Pilot incident as disconfirming pattern, not confirmation | 173, 221 | B 524, B1 row 2 (534) | Yes (whether the submission passed is unstated in both) |
| Panel N ≈ 50, not powered for factor analysis; Study 2 takes it up | 159, 221 | B 517; C 556 | Yes |
| Study 2 N = 200–250 | not stated | C 556 | Body silent (acceptable) |
| Gate binds both parties (reviewer accuracy priced) | 215 | B 488 | Yes |
| Platform assigns reviewers | 215 | B 488 | Yes |
| Rule itself retunes over the term | 215 | B 488; C 554 | Yes — but C 554's "freezing the gate configuration" collides with it; Finding 4 |
| Who retunes; whether it counts as an intervention | not stated | not stated | Gap in both; Finding 4 |
| Exit/escalation rights undocumented, to be catalogued | 215 | B 490 | Yes — but the "drop ≠ termination" point is gone; Finding 8 |
| Merge drift excluded from *keeping track*; Table B1 "states exactly that" | 215 | B1 row 3 (535) — "announcements or compiler updates" | Near-match, not exact; Finding 12 |
| Researcher-blind by procedure; incidental recognition possible | 221 | B 515 | Yes |
| IRB exempt, Protocol 260511078 | 221 | B 517 | Yes |
| Hult, sixteen weeks, spring 2027 | 221 | B 466, 488 | Yes |
| Four CIT modules map to RQ1–4 | 221 | B 496–501 | Yes |
| Analysis is abductive; negative case pre-specified | absent | B 505–511 | Body silent; Finding 9 |
| Strategic research site / hard case | absent | B 472–474 (Trinidad), 490 (Hult) | Body silent; warrant attached to non-corpus cohorts; Finding 7 |
| Nomological predictions "pre-registered" for Study 2 | 159 | C 556 | Same wording; both overstate status; Finding 2 |
| Four nomological relations testable | 159 | C 556–562 operationalize one | **No**; Finding 2 |
| Measurement model | 175 (neither reflective nor formative); 225 (higher-order?) | C 556–562 (per-dimension CFA) | **No** — three models; Finding 3 |
| Study 3 carries dependence, shocks, channel slack, mindlessness, machine heuristic | 107, 129, 185, 221 | C 566 | Yes |
| Proposition 2 → Study 3; Proposition 3 → Study 4 | 199, 201 | C 566, 574 | Yes |
| Proposition 1 → ? | 197 | none | Unassigned; Finding 11 |
| Cohort-level falsifier (attrition, contestation, failures) | 193 | C 568 | Yes in content; no sample; Finding 11 |
| Figure 1 | 177 (placeholder) | — | Still missing |

Every Study 2 and Study 3 pointer in the body resolves to a paragraph in Appendix C. Studies 1 and 4 are never named in the body, which is fine.

---

## Part 3 — What the cut cost

The cut plan set the Empirical Strategy at ~650 words with Appendix B carrying the detail; the result is 703 words in two subsections. Measured against the plan, four things were lost that the plan did not intend to lose, and one thing was lost that it did.

1. **The RQ4 "both" sentence.** Plan: "RQ4's separation rationale in one sentence." Executed: the rationale survived, the sentence naming the primary comparison did not. Cost: Finding 6 — the body reintroduces last round's wavering.
2. **The psychometric-form paragraph.** Plan: reduce to one sentence and move it to Empirical Strategy. Executed: one sentence, left in the construct section (175), and the sentence chosen was the negation ("neither … nor") rather than the positive statement the old paragraph also contained ("psychometrically separable for discriminant testing"). Cost: Finding 3 — the compression turned a division of labor into a contradiction with line 225.
3. **The strategic-site / abductive paragraph.** Plan: "cut … to a parenthetical citation." Executed: removed entirely. Cost: Finding 9 — the body no longer says the analysis is abductive or that a negative case exists.
4. **The "drop a course ≠ account termination" sentence.** Not named in the plan. Cost: Finding 8 — the caveat reads as clerical rather than structural.
5. **Semantic Relations falsifiers.** Plan: one sentence per prediction. Executed as planned, and two failure conditions went with the exposition — a near-zero Spitzberg correlation showing unrelated domains, a Rahman convergence strong enough to collapse the boundary. The compressed list keeps directions and drops what would count against them.

What the cut did **not** cost: the three gate properties, the pilot count, the status paragraph, the researcher-blind wording, the Table B1 pointers, and every Study 2/3 reference survived in full. A reader who stops at line 228 knows where the study is, when it fields, what the author has collected, what the panel cannot do, and what the one pilot incident showed. That reader does not know how transcripts will be analyzed, what the CFA will estimate, or who moves the rule. Those are the additions the body needs, and they total perhaps 150 words.

---

## Part 4 — What is strong

The falsification discipline is the paper's methodological signature, and it improved. Study 1's sufficiency criterion (546) now carries the alternative-casing clause: "Fit alone does not stop the analysis; the alternative-casing pass must also come back empty." Study 2 (552) builds the instrument before it tests it, in Zhou's sequence, and names an invariance condition on pooling (554) with a stated consequence for failure. The HTMT .85 rule (562) can kill a dimension. The negative case at 511 is the right kind of falsifier for a necessity claim. Finding 5 asks to make those kill conditions sharper, not to add them.

The pilot is narrated honestly in both places. Two transcripts, one read informally, one unread; the one incident cuts against the construct and is filed under the disconfirming criterion it matches (173, 221, 524).

The site disclosure is complete on the three properties that matter. Mutual bindingness is stated as a fact about the gate with its mechanism (reviewer accuracy priced); algorithmic assignment is stated flatly; the rule shift is distinguished from substrate churn, and the coding protocol excludes the latter for a reason the paper gives. The merge-drift exclusion (215) is a careful coding decision that a less rigorous design would have missed.

The derivation is now shown rather than announced (165): three properties, three deficits, three operations, with bindingness generating *specifying intent* — the reading two reviewers independently offered last round. The machine-heuristic threat (159) comes with a specific partialling test. And the insider-research framing is correctly built on the core/thesis split, with the developmental cohorts explicitly demoted from corpus to calibration ground (484) — the move most insider-AR papers botch. Finding 7 asks the appendix to honor that demotion in two sentences that currently do not.

---

## Prior-round findings: status

From `review_methodology.md` (2026-08-29), numbered as in its ranked list.

| # | Prior finding | Status |
|---|---|---|
| 1 | Missing scale-development study; pooling across non-stationary cohorts | **Resolved** in Appendix C (552, 554) — with a new tension: the freeze must be of the retuning schedule, not the rule (Finding 4); and the Paper 3 panel's own instrument is still unspecified (Finding 1) |
| 2 | Site-fit "refute" rests on undocumented reviewer assignment; who set the weights; unclaimed ground-truth asset | Reviewer assignment **resolved** (confirmed fact). Who retunes and the accuracy-criterion asset **open** (Finding 4) |
| 3 | Pilot overclaim; unstated pilot N | **Resolved** (173, 221, 521) |
| 4 | Empirical status buried in Appendix B; tense slips | **Resolved** (221) |
| 5 | Confirmation-shaped abductive stopping rule | **Resolved** (546) |
| 6 | "Complete anonymity" overclaim | **Resolved** (221, 515) |
| 7 | RQ4 host inconsistency | Appendices **resolved**; body **regressed** by the cut (Finding 6) |
| 8 | Methods-section agentless passives; "we" in a solo paper | Out of scope this round; noted that Appendix B now uses "I" throughout |
| 9 | Citation apparatus (Riordan, Yurek, Möhlmann, JMIR preprint, typo) | Out of scope; spot-checked — Riordan now "as cited in," Yurek in the list, Möhlmann corrected, boundary cases and preprint removed |
| 10 | Prose uniformity | Out of scope |
| 11 | Polemic escalations ("systematically inverting"; "intrinsic") | **Resolved** at 189 and 482 — but the narrowed 482 claim still asserts elicitation across three regimes with no corpus (Finding 7) |
| 12 | Study 3 sample unspecified; interviewer-agent validity; bindingness stakes gradient; duplicate RQ roadmap | Duplicate roadmap **resolved** (B 454 points to body). Study 3 sample **open** (566: "remain to be specified"). Interviewer-agent validity **open** (Finding 10). Stakes gradient **open** and slightly worse (Finding 8) |
| 13 | Under-welded glosses | Out of scope |

Settled facts from the synthesis — mutual bindingness, algorithmic assignment, the rule itself shifting, pilot count of two — are treated as facts throughout this review and not re-raised.

---

## Top five fixes, ranked

1. **State the measurement model and give the loop a falsifier** (Finding 3; lines 175, 225, 556–562). Three first-order reflective factors, correlated; higher-order structure tested by model comparison in Study 2; recursion as a process claim with an episode-sequence criterion added to Table B1. One paragraph and one table row.

2. **Say what the three-wave panel measures** (Finding 1; lines 221, 517). Provisional items feeding Study 2's pool, behavioral indicators from the gate and repository, or both. Drop "convergence check" until an algorithmacy measure exists at wave 2.

3. **Disclose who retunes the rule, freeze the schedule rather than the rule, and claim the accuracy criterion** (Finding 4; lines 213, 215, 488, 492, 554). This closes the insider-intervention question, rescues the Study 2 pooling fix from contradicting the site description, and adds the one measurement no commercial-platform study can run.

4. **Bring the body's claims down to what Appendix C tests** (Finding 2; line 159 vs. 556–562). One instrumented relation, not four; "to be pre-registered," not "pre-registered"; an equivalence bound for the *Embracing* null; Spitzberg's measure added to Study 2.

5. **Restore three sentences the cut took** (Findings 6, 8, 9; lines 215, 219, 221). RQ4's "separates from both"; "a student's option to drop a course is not the analogue of unilateral account termination," plus the stakes gradient; and two sentences naming the abductive logic and the pre-specified negative case. Roughly 120 words returns the body to stating its own design.
