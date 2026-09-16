# AI Prompt for Deductive Qualitative Analysis of APP Well-Being and Belonging Interviews

A structured prompt for using a large language model (LLM) as a **secondary reviewer** in the qualitative analysis of interviews with critical care Advanced Practice Providers (APPs). The prompt directs the AI to map de-identified interview transcripts onto three predetermined domains and to produce quote tables, summary takeaways, and prioritized system-level recommendations.

**Prompt file:** `QualtitativeInterviewPrompt.md`
**Author:** Katie McCusker, DNP, ARNP, AG-ACNP-BC

---

## Purpose

The prompt was developed for a quality improvement (QI) and program evaluation project that examined workplace well-being and belonging among critical care APPs. The project was prompted by low well-being and belonging scores on an institutional survey.

The prompt was **not** used to replace investigator analysis. The investigator coded all transcripts first using qualitative analysis software. The prompt was then used to generate an independent AI-assisted review, which was compared with the investigator's coding to support **confirmability and trustworthiness**. Where the AI and the investigator disagreed, the investigator's interpretation was retained and the differences were used to check for blind spots and refine the findings.

This approach is consistent with published guidance on using AI in thematic analysis with human oversight (Christou, 2024; Turobov et al., 2024).

---

## Use Case

This prompt may be useful for:

- Nurse, physician, and APP researchers or QI teams analyzing semi-structured interview data
- Projects using **deductive** analysis with domains defined in advance from the literature
- Investigators who want an AI-assisted check on their own coding, particularly in small teams with limited opportunity for multiple human coders
- Projects focused on **system-level or organizational** issues rather than individual or unit-specific concerns

It can be adapted to other populations or topics by replacing the project background and the three predetermined domains.

It is **not** intended as a stand-alone analysis method or as a substitute for human coding and interpretation.

---

## Inputs

| Input | Description |
|---|---|
| Interview transcripts | 13 semi-structured interview transcripts from critical care APPs across multiple ICUs and 3 teams within a single facility, labeled by interview number (Interview 1 through Interview 13) |
| This prompt | The full text of `QualtitativeInterviewPrompt.md`, provided before the transcripts |

**Data protection requirements**

- Transcripts must be **fully de-identified** before being provided to any AI tool. Remove participant names, colleague names, unit names, the institution's name, and any other identifying details.
- Use an AI tool and account whose data terms prevent uploaded content from being shared or used for model training.
- Confirm that AI use is consistent with your IRB or QI determination and your institution's data policies.

Transcripts are **not** included in this repository.

---

## Analytic Framework

The prompt specifies a deductive analysis using three domains drawn from the literature:

1. Mentorship and Professional Development
2. Professional Autonomy and Role Clarity
3. Organizational Support and Recognition

The AI is instructed to:

- Review each transcript systematically for content related to each domain
- Develop sub-categories within each domain based on the interview data
- Retain a sub-category only if it is supported by **at least 3 different interviews**
- Allow a single quote to map to more than one sub-category
- Note frequency, intensity, and contradictory perspectives
- Consider how issues in one domain interact with or worsen issues in another
- Identify whether each issue affects well-being, belonging, or both
- State explicitly if a domain has insufficient supporting data

---

## Prompt Structure

| Section | Content |
|---|---|
| 1. Project Overview | Background, sample, and system-level scope |
| 2. Analytical Approach | Deductive method, coding process, quality criteria, and data-handling rules |
| 3. Deliverables | Specifications for the three output documents |
| 4. Analytical Notes | The AI's role as an initial reviewer, handling contradictions, depth of analysis, and insufficient data |
| Output File Naming | Required file names |

---

## Outputs

| # | File name | Content |
|---|---|---|
| 1 | `APP_Wellbeing_Quotes_by_Theme.docx` | 3 to 5 representative quotes per sub-category, organized by domain, each labeled with its interview number |
| 2 | `APP_Wellbeing_Major_Takeaways.docx` | Bulleted synthesis by domain, with prevalence and links to well-being and/or belonging |
| 3 | `APP_Wellbeing_Recommendations.docx` | 5 to 8 system-level recommendations ranked High, Medium, or Lower priority, each with supporting evidence, expected impact, and linked domain(s) |

---

## How to Use

1. De-identify all transcripts and label each by interview number.
2. Complete your own coding before running the prompt.
3. Open a new session in your chosen AI tool.
4. Paste the full prompt, then provide the transcripts.
5. Save the outputs using the file names above.
6. Record the model name and version, date, and any follow-up instructions given during the session.
7. Compare the AI output with your coding, sub-category by sub-category, noting agreement, differences in frequency, and categories identified by only one reviewer.
8. Verify every AI-provided quote against the original transcript before using it.

AI output is not deterministic. Running the prompt again may produce different sub-categories, wording, or counts.

**Tested with:** Anthropic Claude (model/version: _add here_)

---

## Limitations and Responsible Use

- **Quote accuracy.** AI tools may paraphrase, merge, or misattribute quotes even when instructed to quote verbatim. Check every quote against the source transcript.
- **Frequency counts.** AI-generated counts can differ from investigator counts and should not be reported as findings without verification.
- **Deductive constraints.** Directing the AI to predetermined domains may cause it to miss important findings outside those domains. Investigator review remains essential for identifying unexpected patterns.
- **Terminology.** The prompt uses research terms such as "themes," "codes," and "thematic analysis." QI and program evaluation projects may prefer terms such as "domains," "categories," or "findings" when reporting results.
- **Clinical perspective.** The AI does not bring clinical experience to its interpretation. Adding an instruction for the AI to reason from the perspective of a practicing critical care clinician is a possible refinement for future versions.
- **Human oversight.** AI output is a starting point for comparison, not a final result. Final interpretation rests with the investigator.

---

## References

Christou, P. A. (2024). Thematic analysis through artificial intelligence (AI). *The Qualitative Report, 29*(2), 560–576. https://doi.org/10.46743/2160-3715/2024.7046

Turobov, A., Coyle, D., & Harding, V. (2024). *Using ChatGPT for thematic analysis* [Preprint]. arXiv. https://doi.org/10.48550/arxiv.2405.08828
