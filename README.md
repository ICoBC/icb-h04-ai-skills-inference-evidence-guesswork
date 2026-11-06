<!--
author:   ICoBC - International Council on Badges and Credentials
email:    info@icobc.net
version:  1.0.0
language: en
narrator: UK English Female
comment:  This course explains how AI infers skills from CVs, work activity and content, compares inferred skills with credentialed skills as evidence, and shows when inference may be a high-risk use under the EU AI Act.

@style
:root { --icobc-navy:#02375B; --icobc-orange:#F78222; --icobc-cyan:#5DCAE7; --icobc-lime:#B1CF37; --icobc-mist:#F1F5F8; --icobc-line:#D8E2E9; --icobc-muted:#4F6576; }
body { font-family: "Open Sans", Arial, sans-serif; }
h1, h2, h3, h4 { color: var(--icobc-navy); }
a { color: var(--icobc-navy); }
table th { background: var(--icobc-mist); color: var(--icobc-navy); }
blockquote { border-left: 4px solid var(--icobc-orange); background: var(--icobc-mist); padding: 8px 16px; }
@end
-->

# AI Skills Inference: Evidence or Guesswork?

*Inferred skill profiles compared with credentialed skills.*

Course ID: ICB-H04 | Badge: "AI Skills Inference: Evidence or Guesswork? (Knowledge, L3)" | Alignment code: ICSF-AIRC-L3-K

## About this course

AI tools can read a CV, a project history or a set of learning content and produce a list of skills. Many HR and learning platforms now offer this. The list looks precise. Whether it is good evidence is a different question, and the answer depends on how the list was made and what it is used for.

This course helps you explain how skills inference works, compare it with credentialed skills, and recognise when a use of inference may count as high risk under the EU AI Act.

**Who this course is for**

- HR, talent acquisition and mobility teams (C2)
- HR and learning technology owners (C3)
- Programme and micro-credential leads (E1)
- Policy makers and public agencies (P2)

**Framework alignment**

The course sits in the ICoBC Credentialing Skills Framework (ICSF), skill AIRC "Trustworthy AI in recognition" (VRITE pillar: Trustworthiness), at level L3 "Enable", stage K "Knowledge". At L3 a person designs AI-supported workflows for a programme, sets review points and documents risks. At stage K, the person understands concepts, rules, standards and the reasons behind them, and can explain and recognise. This course teaches and checks that understanding. The quality focus is VRITE Rigor.

**Prerequisite**

ICB-F05 Skills Language 101: Frameworks, Taxonomies and Levels. You should know what a skills taxonomy is and how skill levels are described.

**Learning outcomes**

1. Explain how AI infers skills from CVs, work activity and content.
2. Compare inferred skills with credentialed skills in terms of evidence.
3. Identify when inference may be a high-risk use under the AI Act.

**Workload and format**

Self-paced, 2 hours of notional learning. Live or workshop elements are described in facilitator notes and are optional for self-paced learners.

**Assessment and badge**

You complete a knowledge check with scenarios (10 questions). Passing it earns the badge "AI Skills Inference: Evidence or Guesswork? (Knowledge, L3)". Completing the course shows that you met this knowledge standard. It does not prove competency in a job.

| Outcome | Module | How it is assessed |
|---|---|---|
| 1. Explain how AI infers skills from CVs, work activity and content | How inference works | Module quiz and final knowledge check (scenario questions) |
| 2. Compare inferred skills with credentialed skills in terms of evidence | Evidence quality | Module quiz and final knowledge check (scenario questions) |
| 3. Identify when inference may be a high-risk use under the AI Act | Uses and risks | Module quiz and final knowledge check (scenario questions) |

> Status as of November 2026; check before publishing. Legal dates in this course follow the notes supplied by ICoBC and must be checked against the final published text of the EU AI Act and the Digital Omnibus on AI.

<!-- VERIFY: Confirm the status of the Digital Omnibus on AI and the application dates in the final published text before release. -->

## How inference works

In this module you learn what skills inference is, which data sources feed it, and what steps a typical system follows. You also see where its output can go wrong.

### What skills inference means

Skills inference is a method where software estimates which skills a person has, without the person listing each skill and without an assessor checking each one. The software looks at data about the person and produces a profile: a list of skills, sometimes with levels or confidence scores.

Three terms help here.

- **Self-claimed skill:** the person states the skill, for example in a profile form.
- **Inferred skill:** a system estimates the skill from other data.
- **Verified skill:** a person or body has checked evidence of the skill, for example through assessment or a credential.

Inference sits between claiming and verifying. It is an estimate based on patterns. It is common in HR software and is an emerging practice, so methods, quality and legal treatment still vary widely.

The graphic below shows the spectrum.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Spectrum from self-claimed to inferred to verified skills</title>
  <desc>A horizontal line with three labelled points. Self-claimed skills sit on the left, inferred skills in the middle, and verified skills on the right. Under each point is a short note on who makes the statement and how strong the evidence is.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <text x="400" y="50" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="20" font-weight="bold" fill="#02375B">Three ways a skill enters a profile</text>
  <line x1="100" y1="170" x2="700" y2="170" stroke="#D8E2E9" stroke-width="2"/>
  <circle cx="140" cy="170" r="30" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <circle cx="400" cy="170" r="30" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <circle cx="660" cy="170" r="30" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="140" y="176" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" font-weight="bold" fill="#02375B">1</text>
  <text x="400" y="176" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" font-weight="bold" fill="#02375B">2</text>
  <text x="660" y="176" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" font-weight="bold" fill="#FFFFFF">3</text>
  <text x="140" y="240" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" font-weight="bold" fill="#02375B">Self-claimed</text>
  <text x="400" y="240" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" font-weight="bold" fill="#02375B">Inferred</text>
  <text x="660" y="240" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" font-weight="bold" fill="#02375B">Verified</text>
  <text x="140" y="275" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">The person says it</text>
  <text x="400" y="275" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">A system estimates it</text>
  <text x="660" y="275" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">An assessor checks it</text>
  <text x="140" y="305" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">No check</text>
  <text x="400" y="305" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">Pattern, not proof</text>
  <text x="660" y="305" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">Evidence reviewed</text>
  <text x="400" y="390" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Evidence strength generally increases from left to right</text>
</svg>

### Data sources

Inference systems read different kinds of data. The most common sources are:

- **CVs and profiles:** job titles, employers, education, free text.
- **Work activity:** project records, tickets, code repositories, documents, calendar or collaboration data, performance notes.
- **Content:** course descriptions, learning content a person completed, job advertisements, internal role descriptions.
- **Labour market data:** job postings and occupational data used to learn which skills usually go with which roles.

Each source is a trace of behaviour, not a direct measure of ability. A job title says what a person was called. A ticket history says what a person touched. Neither says how well the person did the work.

### The typical steps

Most systems follow a similar chain.

1. **Extract:** the system finds words and phrases in the text, such as "managed a team of eight" or "built dashboards".
2. **Normalise:** it maps those phrases to entries in a skills taxonomy, for example a list of named skills. This is where your knowledge of taxonomies from ICB-F05 matters.
3. **Infer:** it adds skills that are not written but are likely. For example, if many people with the title "data analyst" also list a certain skill, the system may add that skill to a new data analyst.
4. **Score:** it assigns a level or confidence value.
5. **Output:** it shows a profile, a match to a role or a learning suggestion.

Step 3 deserves attention. The system uses statistics about groups to make claims about an individual. The inferred skill may be common in the group and still absent in the person.

### Where it can go wrong

Several sources of error appear in this chain.

- **Wording:** people describe the same work in different words. Some write more, some less.
- **Taxonomy limits:** the taxonomy may lack a skill, or may split one skill into several.
- **Group bias:** if training data reflects past hiring patterns, the system may repeat them.
- **Stale data:** a skill used five years ago may still appear current.
- **False precision:** a score of 0.82 looks exact, but it does not state how it was reached.

**Worked example: Corporate academy skill profiles**

A corporate academy in a manufacturing company introduces a tool that reads employee profiles and project records and proposes skills. A maintenance planner, whose profile mentions "root cause analysis for line stoppages", receives the inferred skills "problem solving" and "process improvement". She also receives "statistical process control", because many colleagues with similar titles have it. She has never used it.

The academy lead reads the tool's documentation. The first two skills follow from her own words. The third follows from group patterns. The lead decides to label the third skill "suggested" in the profile and to ask the planner to confirm or remove it. This keeps inferred items visible as estimates.

**Worked example: University skills mapping of course content**

A university maps module descriptions to a skills taxonomy using an inference tool, so that students can see skills linked to their studies. A module on "Qualitative research methods" is mapped to "interviewing" and "thematic analysis". The tool also adds "data visualisation", because the module handout mentions "presenting findings". The programme lead checks the learning outcomes and assessment tasks and finds that no outcome covers visualisation. She removes the skill from the mapping.

Notice what each example shows. The first concerns a person. The second concerns content. In both, a human review step caught an item the system had added without support.

**Practice activity: Trace an inferred skill**

Take a CV or a profile of your own, or a short sample your facilitator provides. Choose three skills that a system could infer from it. For each one, write down:

1. Which words or data would trigger the skill.
2. Whether the skill is stated, implied by the text, or implied by group patterns.
3. What other evidence would show the skill is real.

Keep your notes. You will reuse them in the next module.

<details>
<summary>Facilitator notes</summary>

Optional live element (30 minutes). Give each pair a short fictional CV. Ask them to act as the "extraction step" and underline phrases, then act as the "inference step" and list skills they would add based on typical patterns for the job title. Compare lists across pairs. Discuss why lists differ and what that says about the stability of inference. Remind participants that all CVs used must be fictional or fully anonymised.

</details>

### Check your understanding

**Question 1.** Which description fits an inferred skill best?

[( )] A skill the person typed into a profile form.
[(X)] A skill a system estimates from data such as a CV, work records or content.
[( )] A skill an assessor confirmed after reviewing evidence.
[( )] A skill listed in a job advertisement.
[[?]] Think about who or what makes the statement.
****
An inferred skill is estimated by a system from other data. A typed skill is self-claimed, and a confirmed skill is verified.
****

**Question 2.** A system adds the skill "budget forecasting" to a profile because many people with the same job title list it. The person's CV does not mention it. What does this show?

[( )] The person has been assessed on budget forecasting.
[( )] The CV was read incorrectly.
[(X)] The system used group patterns to make a claim about an individual.
[( )] The taxonomy is complete.
[[?]] The skill is not in the CV. Where else could the claim come from?
****
Adding a skill that is not in the person's data uses statistics about a group. The skill may be common in the group and still absent in the person.
****

**Question 3.** Which data source is a direct measure of how well a person performs a skill?

[( )] A job title.
[( )] A list of projects a person worked on.
[( )] A course description the person completed.
[(X)] None of these is a direct measure of performance.
[[?]] Consider what each source records: names, activity or content.
****
Titles, activity records and content are traces of behaviour or context. They do not measure how well the work was done.
****

**Question 4.** In a typical inference chain, what happens in the "normalise" step?

[( )] The system adds likely skills based on group patterns.
[(X)] The system maps extracted phrases to entries in a skills taxonomy.
[( )] The system assigns a confidence score.
[( )] The system shows a role match to the user.
[[?]] Think of the link to skills taxonomies from ICB-F05.
****
Normalising maps free-text phrases to named skills in a taxonomy. Adding likely skills is the inference step, and scoring and output come later.
****

## Evidence quality

In this module you compare inferred skills with credentialed skills. You learn to ask what evidence sits behind a skill statement and who stands behind it.

### What counts as evidence

In recognition work, a skill statement is only as strong as the evidence behind it. Evidence is information that supports the claim that a person has a skill. Useful questions are:

- **What was observed or produced?** A work sample, a performance in a task, a test result.
- **Who judged it?** A trained assessor, a peer, a system.
- **Against which standard?** A published skill description, level and criteria.
- **When?** Recent or old.
- **Can it be checked?** Is there a record that another party can verify?

A credentialed skill, such as one linked to a badge or certificate, normally comes with answers to these questions. A credential is issued by a named body, tied to defined criteria, and usually records an assessment or other evidence. Its quality still varies. Credentials differ in rigour, so you must still check the issuer and the assessment method.

An inferred skill usually answers these questions weakly. The system looked at traces, applied a model and produced an estimate. There may be no standard, no judge you can name and no record of reasoning you can inspect.

### Comparing the two

The graphic shows the main comparison points.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Inferred skills and credentialed skills compared by evidence</title>
  <desc>Two columns. The left column, labelled inferred skills, lists four evidence questions with typical answers: traces of activity, a model, often unclear criteria, and variable recency. The right column, labelled credentialed skills, lists the same four questions with typical answers: assessed work, a named issuer, published criteria, and a dated record.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <rect x="40" y="40" width="340" height="50" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="210" y="72" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" font-weight="bold" fill="#02375B">Inferred skills</text>
  <rect x="420" y="40" width="340" height="50" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="590" y="72" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" font-weight="bold" fill="#02375B">Credentialed skills</text>
  <rect x="40" y="110" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="210" y="146" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">What: traces of activity or text</text>
  <rect x="420" y="110" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="590" y="146" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">What: assessed work or performance</text>
  <rect x="40" y="190" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="210" y="226" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Who: a model, often hard to inspect</text>
  <rect x="420" y="190" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="590" y="226" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Who: a named issuer and assessor</text>
  <rect x="40" y="270" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="210" y="306" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Standard: often unclear or internal</text>
  <rect x="420" y="270" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="590" y="306" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Standard: published criteria and level</text>
  <rect x="40" y="350" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="210" y="386" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Record: may change when data changes</text>
  <rect x="420" y="350" width="340" height="60" rx="6" fill="#F1F5F8" stroke="#D8E2E9" stroke-width="2"/>
  <text x="590" y="386" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Record: dated and checkable</text>
</svg>

### Reading the comparison fairly

The comparison does not mean that credentials are always strong and inference is always weak. Some credentials rest on thin assessment. Some inference systems are carefully built, tested against assessed samples and transparent about error rates. What matters is that you can ask the evidence questions and get answers.

Three practical points follow.

1. **Label the type.** A profile that mixes self-claimed, inferred and verified skills should show which is which. Users and decision makers then know how much weight each skill can carry.
2. **Match the claim to the decision.** A rough estimate may be fine to suggest learning content. It is a weak basis for a hiring or promotion decision.
3. **Use inference to point to evidence.** An inferred skill can be a prompt: "This person may have this skill. Where is the proof?" The next step is to find or collect evidence, for example through assessment or recognition of prior learning.

Rigor, the VRITE quality focus of this course, applies here. Rigor means the claim is backed by a defined method, a standard and a record that others can examine.

**Worked example: HR department internal mobility**

An HR department runs an internal mobility platform. It infers skills from employee profiles and project records and matches employees to open roles. A talent partner notices that a project manager in the logistics team is matched to a data governance role. The match rests on an inferred skill, "data quality management", drawn from project notes.

The talent partner does not treat the match as a finding. She asks the employee to share evidence: a document she wrote, or a micro-credential if she has one. The employee shares a data quality checklist she created and a short assessed course she completed last year. The partner now has a self-described work sample and a credential. The inferred skill has led to evidence.

**Worked example: Training provider recognising prior learning**

A training provider receives an application for a short programme from a learner with five years of site supervision. The provider's system infers skills from the learner's CV, including "risk assessment". The admissions lead uses the output to decide what to ask. She invites the learner to submit a risk assessment he wrote and to attend a short interview with a trained assessor. The inferred skill guides the conversation. The assessor's judgement, against the programme's published criteria, decides whether prior learning is recognised.

**Practice activity: Evidence questions grid**

Return to the three skills you chose in the previous module. Draw a grid with five rows: what was observed, who judged it, against which standard, when, can it be checked. For each of the three skills, answer the five questions twice: once for the inferred skill as you imagine it appears in a profile, and once for a credentialed version of the same skill, such as a badge for it. Mark where the answers differ most.

<details>
<summary>Facilitator notes</summary>

Optional live element (30 minutes). Provide three fictional profile entries, one self-claimed, one inferred and one verified by a badge with published criteria. Ask small groups to rank them by evidence strength and justify the ranking using the five evidence questions. Then give each group a decision (suggest a course, shortlist for interview, award a promotion) and ask which entry types are acceptable for each. Expect disagreement. Use it to show that the acceptable evidence level depends on the decision.

</details>

### Check your understanding

**Question 1.** Which question helps you judge the strength of evidence behind a skill statement?

[( )] How many skills does the profile list?
[( )] How modern does the interface look?
[(X)] Who judged the skill, and against which standard?
[( )] How long is the profile?
[[?]] Think about who stands behind the claim.
****
Evidence strength depends on what was observed, who judged it, against which standard, when and whether it can be checked.
****

**Question 2.** A hiring manager sees a profile where all skills appear in one list with no labels. What is the main problem?

[( )] The list is too short.
[(X)] The reader cannot tell self-claimed, inferred and verified skills apart.
[( )] Credentials should never appear in profiles.
[( )] Inferred skills should never appear in profiles.
[[?]] Consider what the reader needs to know to weigh each item.
****
Without labels, the reader cannot tell how much weight each skill deserves. Showing the type of each skill supports fair use.
****

**Question 3.** Which statement about credentialed skills is the most accurate?

[( )] All credentials rest on strong evidence.
[( )] Credentials never need checking.
[(X)] Credentials normally come with an issuer, criteria and a record, but their rigour still varies.
[( )] Credentials are less reliable than inferred skills.
[[?]] Credentials are structured, but not all are equal.
****
A credential normally names its issuer and criteria and keeps a record. You still check the issuer and the assessment method.
****

**Question 4.** An admissions lead at a training provider uses inferred skills from a CV to decide which evidence to request from an applicant. What role does inference play here?

[( )] It replaces assessment.
[(X)] It points to skills where evidence should be sought.
[( )] It confirms the skills as verified.
[( )] It removes the need for published criteria.
[[?]] The assessor still decides.
****
Used as a prompt, inference guides where to look for evidence. The decision rests on the evidence and the published criteria.
****

**Question 5.** Which decision is the weakest fit for an unverified inferred skill as the only evidence?

[( )] Suggesting an optional learning course.
[( )] Prompting a conversation about experience.
[(X)] Rejecting a candidate or denying a promotion.
[( )] Ordering a list of suggestions for the person to review.
[[?]] Consider which decision carries the highest consequences for a person.
****
The higher the consequence of a decision for a person, the stronger the evidence should be. Rejection or denial of promotion needs more than an unverified estimate.
****

## Uses and risks

In this module you learn how inference is used in HR and education, what risks arise, and when a use may be high risk under the EU AI Act.

### Common uses

Skills inference appears in several settings.

- **Talent acquisition:** screening applicants, ranking candidates, matching them to roles.
- **Internal mobility:** suggesting roles, projects or mentors to employees.
- **Workforce planning:** estimating the skills an organisation has and lacks.
- **Learning:** recommending courses, mapping content to skills.
- **Education:** mapping modules to skills, supporting recognition of prior learning, guiding students.
- **Public agencies:** matching job seekers to vacancies or training.

These uses differ in the effect on a person. A course suggestion has a small effect. A ranking that decides who is invited to interview has a larger effect.

### Risks to manage

Risks follow from what you learned in Modules 1 and 2.

- **Unfair outcomes:** if the system learned from biased data, it may favour some groups and disadvantage others.
- **Opacity:** users may not know a system was used or how it reached a result.
- **Errors:** wrong or missing skills can lead to wrong matches.
- **Over-reliance:** reviewers may treat a score as fact.
- **Data protection:** profiles can include personal data and, in some cases, special categories of data. Data protection rules apply alongside AI rules.

An L3 practitioner designs a workflow that reduces these risks. That means setting review points, assigning a named human reviewer, keeping a record of decisions and documenting risks and limits.

### The EU AI Act in brief

The EU AI Act is a regulation that sets rules for AI systems based on risk. It uses categories. Some practices are prohibited. Some systems are classed as high risk and must meet requirements. Others have lighter duties such as transparency.

Under the AI Act, Annex III lists areas where AI systems may be high risk. These include certain uses in employment and worker management, and certain uses in education and vocational training. The detail matters: the question is whether the system is used for the listed purposes, not simply whether it is called an "AI skills tool".

<!-- VERIFY: Check the exact wording of the Annex III employment and education entries in the final published text before using specific references. -->

For employment, the listed purposes include uses such as recruitment and selection, and decisions that affect the terms, promotion or termination of work relationships, or the allocation of tasks or the monitoring and evaluation of workers. For education and training, they include uses such as deciding access or admission, evaluating learning outcomes, and assessing the level of education a person will receive.

So skills inference is not high risk in every case. It may be high risk when its output is used for employment decisions or for the listed education purposes. The same tool used only to suggest optional learning may fall outside those purposes. Context of use decides.

### Timing

According to ICoBC's notes, under the AI Omnibus (provisional agreement of 7 May 2026), obligations for Annex III high-risk systems apply from 2 December 2027, and obligations for Annex I product-embedded systems apply from 2 August 2028. These dates come from a provisional agreement.

> Status as of November 2026; check before publishing. Check the final published text of the AI Act and the Digital Omnibus on AI for the dates and for the exact scope of the Annex III entries.

<!-- VERIFY: Confirm the final dates and scope against the Official Journal of the European Union. -->

Organisations should not wait for the dates. Good practice such as human review, documentation and evidence labelling reduces risk now, and it prepares the organisation for later obligations.

### A simple screening approach

When you review a use of inference, ask three questions.

1. **Purpose:** what decision does the output feed into?
2. **Effect:** does the decision affect a person's access to work, promotion, task allocation, education or training?
3. **Role of the output:** does the output decide, strongly influence or only inform?

If the purpose is in an employment or education area of the kind listed in Annex III, treat the use as potentially high risk and seek legal and compliance advice. A screening is not a legal opinion. It helps you decide when to escalate.

<svg viewBox="0 0 800 450" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Screening questions for high-risk use of skills inference</title>
  <desc>A vertical flow of three questions. The first asks what decision the output feeds into. The second asks whether the decision affects access to work, promotion, task allocation, education or training. The third asks whether the output decides, strongly influences or only informs. An arrow leads to a box that says treat as potentially high risk and seek legal and compliance advice, and another box that says document the use and keep human review.</desc>
  <rect x="0" y="0" width="800" height="450" fill="#FFFFFF"/>
  <rect x="220" y="20" width="360" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="56" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">1. What decision does the output feed?</text>
  <line x1="400" y1="80" x2="400" y2="110" stroke="#02375B" stroke-width="2"/>
  <rect x="220" y="110" width="360" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="134" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">2. Does it affect access to work, promotion,</text>
  <text x="400" y="154" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">task allocation, education or training?</text>
  <line x1="400" y1="170" x2="400" y2="200" stroke="#02375B" stroke-width="2"/>
  <rect x="220" y="200" width="360" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="236" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">3. Decides, strongly influences or informs?</text>
  <line x1="320" y1="260" x2="190" y2="310" stroke="#02375B" stroke-width="2"/>
  <line x1="480" y1="260" x2="610" y2="310" stroke="#02375B" stroke-width="2"/>
  <rect x="40" y="310" width="300" height="100" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
  <text x="190" y="345" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" font-weight="bold" fill="#02375B">Possible high-risk use</text>
  <text x="190" y="370" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Seek legal and compliance advice</text>
  <rect x="460" y="310" width="300" height="100" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="610" y="345" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" font-weight="bold" fill="#02375B">Lower consequence use</text>
  <text x="610" y="370" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Still document and keep review</text>
</svg>

**Worked example: Corporate recruitment screening**

A talent acquisition team in a large company wants to use a tool that infers skills from CVs and ranks applicants for each vacancy. The recruiter would see the top 20 from several hundred applications and invite only those. The team lead applies the three questions. The decision is who is invited to interview. This affects access to work. The ranking strongly influences who is seen. The team lead concludes that this use may be high risk under the AI Act, flags it to legal and compliance, and pauses the rollout until a review is done. In the meantime she asks for a design with named human reviewers, a record of why each candidate was advanced or not, and a way for candidates to request human review.

**Worked example: University course recommendations**

A university adds a feature that infers skills from a student's completed modules and suggests optional elective modules. The student sees the suggestions and chooses freely. Admissions, assessment and progression are not affected. The programme lead applies the three questions. The decision is which optional module the student picks. The output only informs. She considers this a lower-consequence use. She still documents the purpose, the data used and the limits, labels the suggestions as "suggested from your completed modules" and keeps a feedback button so students can report wrong suggestions. She notes that if the feature later influenced admission or assessment, she would re-screen it.

**Practice activity: Screen three uses**

Write down three uses of skills inference in your own organisation or a fictional one. For each, answer the three screening questions. Then mark each use as "possible high risk, escalate" or "lower consequence, document and review". For each, name the human reviewer and one review point you would set.

<details>
<summary>Facilitator notes</summary>

Optional live element (45 minutes). Run a risk workshop with mixed roles (HR, learning technology, programme lead, policy). Give each table two scenario cards. Tables complete the screening questions and a one-page risk note: purpose, data, reviewer, review point, known limits, escalation route. Each table presents to the room. Remind participants that this is a learning exercise. The screening does not replace legal advice, and the final legal text must be checked. Encourage participants to bring one real use case to the next session if their employer permits.

</details>

### Check your understanding

**Question 1.** When may a skills inference system fall under high-risk use in the AI Act?

[( )] Whenever it uses any kind of AI.
[( )] Only when it is sold outside the EU.
[(X)] When its output is used for purposes listed in Annex III, such as employment decisions.
[( )] Never, because skills are not personal data.
[[?]] The purpose of use matters more than the label of the tool.
****
Annex III lists areas of use, including certain employment and education purposes. Context of use decides whether a system may be high risk.
****

**Question 2.** An organisation uses skills inference only to suggest optional learning courses that employees can ignore. Which statement fits best?

[( )] It is automatically prohibited.
[(X)] It is likely a lower-consequence use, but it still needs documentation and review.
[( )] It requires no documentation at all.
[( )] It is the same as automated rejection of applicants.
[[?]] Check what decision the output feeds and who decides.
****
The output informs an optional choice and does not affect access to work or promotion. Good practice still asks for documentation and review.
****

**Question 3.** What does ICoBC's note say about the application date for Annex III high-risk obligations under the AI Omnibus (provisional agreement of 7 May 2026)?

[( )] They apply from 1 January 2025.
[( )] They apply from 2 August 2028.
[(X)] They apply from 2 December 2027.
[( )] They have no application date.
[[?]] Annex I product-embedded systems have a different, later date.
****
The note gives 2 December 2027 for Annex III and 2 August 2028 for Annex I. These come from a provisional agreement, so check the final published text.
****

**Question 4.** Which review design best reduces the risk when inference supports a promotion decision?

[( )] Accept the highest-scoring employee automatically.
[( )] Hide the use of the tool from employees.
[(X)] Name a human reviewer, set review points, record decisions and document risks and limits.
[( )] Remove all skill data from the process.
[[?]] An L3 practitioner designs workflows with review points and documentation.
****
Human review with named responsibility, records and documented risks is the design the L3 skill describes. Hiding the tool or accepting scores automatically increases risk.
****

## Assessment and badge

This is the final knowledge check with scenarios. It has 10 questions that cover all three learning outcomes. Each question has four options and one correct answer. Read each scenario carefully before you answer.

**Pass rule:** you pass with at least 8 of 10 questions correct (80 per cent). You may retake the check. Read the explanations after each question.

**Badge evidence:** a passed knowledge check. Passing leads to the badge "AI Skills Inference: Evidence or Guesswork? (Knowledge, L3)", alignment code ICSF-AIRC-L3-K. The badge records that you met the knowledge standard of this course. It does not prove competency in a job.

**Rubric**

| Criterion | Meets the standard | Does not yet meet the standard |
|---|---|---|
| Outcome 1: Explain how AI infers skills | Answers at least 3 of 4 related questions correctly, showing understanding of data sources, steps and limits | Fewer than 3 of 4 correct |
| Outcome 2: Compare inferred and credentialed skills | Answers at least 3 of 4 related questions correctly, showing understanding of evidence questions and labelling | Fewer than 3 of 4 correct |
| Outcome 3: Identify possible high-risk use | Answers at least 2 of 2 related questions correctly, showing understanding of purpose, effect and timing notes | Fewer than 2 of 2 correct |
| Overall pass rule | At least 8 of 10 correct and each outcome criterion met | Below 8 of 10 or any outcome criterion not met |

### Final knowledge check

**Question 1.** A talent acquisition specialist reads that a tool "extracts and normalises" skills from CVs. What does "normalise" mean in this context?

[( )] The tool deletes duplicate CVs.
[(X)] The tool maps phrases in the CV to named skills in a taxonomy.
[( )] The tool corrects spelling errors only.
[( )] The tool assigns each person an average score.
[[?]] Think of taxonomies from the prerequisite course.
****
Normalising maps free-text phrases to named skills in a taxonomy, so that different wordings point to the same skill.
****

**Question 2.** A learning technology owner sees that a system added the skill "stakeholder negotiation" to a profile. The employee's CV and records never mention negotiation, but colleagues with the same job title often list it. Where did this skill most likely come from?

[( )] From an assessor who observed the employee.
[( )] From the employee's own claim.
[(X)] From group patterns used to infer skills for people with similar titles.
[( )] From a published credential.
[[?]] The skill is not in the employee's data.
****
Skills that do not appear in the person's own data but are common in a group are added through group-level patterns. They are estimates about the individual.
****

**Question 3.** A programme lead at a college receives a mapping of course content to skills made by an inference tool. Which step best protects the quality of the mapping?

[( )] Publish it immediately because it is automated.
[( )] Remove all human review to save time.
[(X)] Check each mapped skill against the course's learning outcomes and assessment tasks.
[( )] Add more skills until the mapping looks full.
[[?]] The evidence for a skill in a course is in what students must do and show.
****
Learning outcomes and assessment tasks show what students actually do and are assessed on. Checking against them catches skills the tool added without support.
****

**Question 4.** An HR team member says, "The tool gives scores such as 0.87, so the skill level is exact." What is the best response?

[( )] Agree, because numbers are always precise.
[(X)] Explain that a score is a model estimate and does not by itself say how it was derived or how reliable it is.
[( )] Say that scores are always wrong.
[( )] Say that only scores below 0.5 matter.
[[?]] Think about false precision.
****
A numerical score can look exact. It is an estimate from a model, and its reliability depends on the data, method and testing behind it.
****

**Question 5.** A mobility team compares two entries for the skill "project risk assessment": one inferred by a system from project notes, and one linked to a badge with published criteria, a named issuer and an assessed work sample. Which statement is most accurate?

[( )] The inferred entry has stronger evidence because it uses more data.
[( )] Both entries have the same strength of evidence.
[(X)] The badge entry normally has stronger evidence because it has a named issuer, criteria and an assessment record.
[( )] Neither entry can be used for any purpose.
[[?]] Use the five evidence questions: what, who, standard, when, check.
****
A credential with an issuer, criteria and assessed work typically answers the evidence questions better. Its rigour still depends on the issuer and method.
****

**Question 6.** A university lead wants to use inferred skills when reviewing applications for a programme with limited places. A colleague suggests treating the inferred skills as verified. What is the best advice?

[( )] Treat them as verified because they come from software.
[(X)] Label them as inferred, use them to prompt requests for evidence, and rely on assessed evidence and published criteria for the decision.
[( )] Remove all skills data from the process.
[( )] Ask applicants to confirm the skills with a tick box and treat that as verification.
[[?]] A tick box is self-claiming, not verification.
****
Inferred skills can guide where to look for evidence. Decisions about places need assessed evidence and published criteria, and the output should be labelled as inferred.
****

**Question 7.** A profile shows self-claimed, inferred and verified skills in one list with no labels. Which change best improves fairness and rigour?

[( )] Shorten the list.
[( )] Sort skills alphabetically.
[(X)] Show the type of each skill (self-claimed, inferred or verified) next to it.
[( )] Remove the verified skills.
[[?]] The reader needs to know how much weight each item deserves.
****
Labelling the type lets readers weigh each skill by the strength of evidence behind it.
****

**Question 8.** A company plans to use skills inference to rank applicants and show recruiters only the top candidates for interview. How should the HR owner treat this use under the AI Act?

[( )] As clearly outside the Act, because it only ranks.
[( )] As prohibited in every case.
[(X)] As a use that may be high risk because it feeds a recruitment decision, so escalate for legal and compliance review.
[( )] As a use that needs no review because the recruiter makes the final call.
[[?]] Consider the purpose, the effect on access to work and how strongly the output influences the outcome.
****
Ranking applicants feeds recruitment and selection, an employment purpose of the kind listed in Annex III. Strong influence on who is seen means the use should be escalated for review.
****

**Question 9.** A policy officer asks when Annex III high-risk obligations apply under the AI Omnibus, according to the course notes. What is the best answer?

[( )] From 2 August 2028, and the date is final.
[(X)] From 2 December 2027 under the provisional agreement of 7 May 2026, with the final published text to be checked.
[( )] From 1 January 2025 under the original Act.
[( )] There is no date and no obligation.
[[?]] The date comes from a provisional agreement.
****
The course notes give 2 December 2027 for Annex III under the provisional agreement of 7 May 2026. Check the final published text for confirmation.
****

**Question 10.** A university offers a feature that infers skills from completed modules and suggests optional electives. Students can ignore the suggestions, and the feature does not affect admission, assessment or progression. What is the best approach?

[( )] Treat it as high risk under Annex III without further thought.
[( )] Skip all documentation because it is low consequence.
[(X)] Document purpose, data and limits, label suggestions as inferred, offer feedback, and re-screen if the use changes.
[( )] Make the suggestions mandatory.
[[?]] A change of purpose can change the risk.
****
The output only informs an optional choice, so the consequence is lower. Documentation, labelling and review remain good practice, and a change in purpose calls for a new screening.
****

## Sources and further reading

Status as of November 2026; check before publishing.

Only sources whose existence is certain are listed. Check the current version and status of each before you rely on it.

- **Regulation (EU) 2024/1689 (Artificial Intelligence Act).** Official text, published in the Official Journal of the European Union. Search for the regulation number on EUR-Lex, the official portal for EU law.
- **Digital Omnibus on AI.** European Commission legislative proposal and the related legislative procedure. Check the European Commission and EUR-Lex for the final published text and the status of the provisional agreement of 7 May 2026.
- **Regulation (EU) 2016/679 (General Data Protection Regulation).** Official text on EUR-Lex. Relevant where inference processes personal data.
- **ESCO (European Skills, Competences, Qualifications and Occupations).** European Commission classification of skills and occupations. Useful as an example of a skills taxonomy.
- **European Qualifications Framework (EQF).** European Union reference framework for qualification levels.
- **ICoBC Credentialing Skills Framework (ICSF).** Published by the International Council on Badges and Credentials (ICoBC). See the ICoBC website for the current version.
- **ICB-F05 Skills Language 101: Frameworks, Taxonomies and Levels.** ICoBC prerequisite course in the Kursbibliothek.

<!-- VERIFY: Add exact EUR-Lex links and citation details only after checking them against the official portal. -->
