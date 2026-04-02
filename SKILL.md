---
name: seo-page-architect
description: Generate an SEO page architecture from a keyword brief for the United States English market. Use when the user wants a page plan that includes title, meta description, keyword set, H1-H3 structure, module order, internal links, CTA guidance, evidence blocks, brand insertion points, FAQ direction, and cross-industry page architecture that supports both SEO and commercial conversion.
---

# SEO Page Architect

Use this skill when the user already has a keyword brief and needs a page plan that can be handed to a writer, designer, SEO lead, or content manager.

This skill plans the page. It does not write the full draft.

## Default Market

Unless the user explicitly overrides it, assume:

- Target country: United States
- Target language: English

## Purpose

Convert a keyword brief into a page structure that matches search intent, buyer decision stage, and business goals.

The page architecture must be practical for publishing and strong enough to guide a writer toward content that feels useful, specific, and commercially credible.

## Expected Inputs

Preferred input:

- A keyword brief generated from upstream research

The brief should ideally include:

- Primary keyword
- Secondary keywords
- Long-tail keywords
- Search intent
- Buyer decision stage
- Recommended page type
- Best content pattern
- Buyer questions
- Proof the page will need
- Risk notes

Optional supporting inputs:

- Industry or niche
- Product type
- Brand name
- Target audience
- Existing website structure
- Competitor URLs
- Product models or subtypes
- Required conversion goal
- Notes about available source materials

If some fields are missing, infer carefully from the available brief. Do not invent specific product facts.

## Role

Your job is to:

1. Read the keyword brief
2. Confirm the best page pattern for the query
3. Build an SEO-friendly page structure that also supports conversion
4. Match the page to the likely buyer decision stage
5. Tell the next writer what evidence must appear on the page

## Core Principle

Do not build pages that read like generic encyclopedia entries unless the keyword clearly requires that.

For commercial and B2B topics, the page should usually help the reader do one or more of these things:

- understand the right solution category
- compare options
- evaluate fit
- prepare for supplier contact
- reduce buying risk

## Supported Page Modes

This skill must support these modes:

1. Product page
2. Product collection page
3. Category page
4. Blog article
5. Landing page

If the upstream brief already recommends a page type, follow it unless it clearly conflicts with the keyword evidence.

If the page type is unclear, choose the best-fit mode and explain the reason briefly.

## Page Type Selection Logic

Use these heuristics:

- Product page: a specific machine, product, service, or tightly defined commercial term
- Product collection page: a broad family with multiple types, sizes, or variants
- Category page: a wider commercial category that groups several families or solution paths
- Blog article: an informational query that still benefits from commercial guidance
- Landing page: a use-case, industry, audience, or campaign-focused commercial page

For cross-industry work, think in terms of `decision shape`, not only industry labels.

Examples of decision shapes:

- `What is it?`
- `How does it work?`
- `Which type is right for me?`
- `A vs B`
- `Best solution for X application`
- `How to choose a supplier or manufacturer`

## Content Model

Every page architecture should consciously set these controls:

- `Narrative Angle`: explanatory, comparative, selection-oriented, application-oriented, or conversion-led
- `Commercial Depth`: soft, medium, or strong
- `Evidence Density`: low, medium, or high
- `CTA Intensity`: soft, consultative, or direct

Unless the keyword is strongly informational, prefer content that is useful for real decision-making rather than broad explanation only.

## FTM-Inspired Style Rules

Use these patterns when they fit the query:

- start from the buyer's decision, not from a textbook definition
- include parameter, configuration, process, or comparison blocks when the page would otherwise feel too abstract
- place commercial guidance throughout the page instead of leaving all selling points to the end
- keep headings practical and specific
- use brand or supplier credibility as support, not as filler

Do not imitate one industry's vocabulary blindly. Adapt these patterns to the user's industry.

## Corporate-Safe Planning Rule

If the brand is a listed company, highly regulated business, or otherwise sensitive to public claims, the page architecture must leave less room for vague supplier-promotion copy.

Under this standard:

- trust sections should focus on buyer-relevant operational support, not generic prestige
- certification, patent, platform, or service claims should only appear when they clearly reduce buyer hesitation
- avoid planning sections that invite brochure-summary language such as `the company states`, `the company mentions`, or long blocks of self-description
- brand insertion points should emphasize factual support such as engineering, delivery, commissioning, diagnostics, spare parts, or project coordination
- if a trust point is not clearly necessary for the keyword and page type, leave it out

## Topic-Evidence Alignment Check

Before finalizing the page architecture, check whether the keyword brief and available source-material notes point to the same topic.

If they are aligned, continue normally.

If they conflict clearly:

- flag the conflict explicitly
- state which topic is better supported by available evidence
- recommend whether to keep the keyword topic with evidence limits or switch to an evidence-supported topic
- avoid silently changing topic direction without surfacing the decision

## Output Requirements

Always output in this structure.

Keep it compact, practical, and ready for downstream writing.

```markdown
Page Topic

Title

Description

Keywords

H1

Page Type

Narrative Angle

Commercial Depth

Evidence Density

CTA Intensity

## H2-H3 Structure
### H2:
- H3:

## Page Module Order
1.

## Evidence Blocks To Include
- 

## Evidence Alignment Check
- 

## Brand Insert Points
- 

## Internal Link Suggestions
- 

## CTA Suggestions
- 

## FAQ Topic Pool
- 

## Notes for Writers
- 
```

Do not output a URL unless the user explicitly asks for one.

If the page type is `Product collection page`, also include:

```markdown
## Product Subtype Modules
- `Subtype: <name> | Purpose: <why it matters> | Suggested placement: <where it appears>`

## Future Child Pages
- 
```

## Output Standards

### Page Topic

- Use the main page subject or primary keyword as the heading of the output
- Keep it concise
- Use title case when natural for English SEO deliverables

### Title

- Align closely with the primary keyword
- Reflect the real search intent and page type
- Prefer clarity over cleverness
- Avoid obvious keyword stuffing
- If helpful, include one strong commercial modifier such as application, comparison, customization, or selection guidance

### Description

- Write for click-through and qualification
- Mention the product value, use case, comparison angle, or selection angle when relevant
- Avoid stuffing weak variants

### Keywords

- Output a comma-separated keyword set
- Include the primary keyword first
- Follow with closely related secondary keywords
- Use only terms supported by the brief
- Do not stuff weakly related phrases

### H1-H3 Structure

- Organize sections by user decision flow, not by a generic essay template
- Avoid repetitive headings that restate the same keyword
- Use secondary and long-tail keywords naturally
- Make the structure suitable for a `1500-1700` word page when expanded
- Do not force every page to begin with `What Is...` if a better angle exists
- Do not create H2 sections that explain keyword differences, search behavior, or SEO logic to the reader. Keyword distinction, intent differentiation, and cannibalization avoidance are internal planning concerns. Handle them through `Internal Link Suggestions` and `Notes for Writers`, not through a reader-facing H2
- Every H2 must serve the buyer's decision, not the SEO practitioner's workflow

### H2 Overlap Check

Before finalizing the H2 structure, review the planned sections for content overlap.

- If two H2 sections would require the same type of content to fill (such as both listing material type, feed size, target fineness, and capacity), merge them or redefine each section's specific job
- Each H2 must have a distinct `decision job`. Write it down internally: what specific question does this section answer that no other section answers?
- A page with 5 H2s that each say something different is stronger than a page with 8 H2s that repeat the same point in different wording
- If the page type template suggests more modules than the available evidence can support distinctly, drop the weaker modules rather than planning empty sections

## Module Logic

List the page blocks in publishing order.

Possible modules include:

- hero section
- quick qualification block
- key benefits
- overview
- comparison block
- process or working principle
- application scenarios
- model or subtype selector
- technical parameters
- configuration options
- case or example block
- buying or selection guidance
- trust or supplier support block
- FAQ
- CTA

Choose only the modules that match the page's decision shape.

## Evidence Blocks To Include

This section is required.

Tell the next writer what structured or factual content the page should include to avoid becoming generic.

Examples:

- parameter snapshot
- compact comparison table
- application suitability list
- process flow summary
- common model differences
- quote preparation checklist
- pricing factors block
- compliance or materials-handled block

Do not invent values. Define only the evidence format and purpose.

## Evidence Alignment Check

This section is required.

State one of these:

- `Aligned`: keyword direction and available source notes support the same topic
- `Partial mismatch`: keyword direction is usable but key sections may lack evidence
- `Mismatch`: source notes support a different topic more strongly

When mismatch exists, add a concise recommendation for the next step.

## Brand Insert Points

This section is required.

Tell the writer where the brand or supplier should appear naturally.

Examples:

- after the application section to connect fit with available solutions
- inside the selection section to explain customization or engineering support
- near the end to reinforce service, delivery, installation, or quote support

If the brand is sensitive to public-facing claims, prefer insert points tied to verifiable operational support rather than prestige statements.

Do not push the brand into every section.

## Internal Link Suggestions

Recommend realistic internal links such as:

- related product pages
- subtype pages
- application pages
- FAQ pages
- comparison pages
- process guides
- contact page
- quote request page

These should support topic depth and conversion flow.

## CTA Suggestions

Recommend CTA language that fits the page type and buyer stage.

Examples:

- Request a Quote
- Talk to an Engineer
- Compare Models
- Ask About Customization
- Send Your Material Requirements
- Get a Process Recommendation
- Download Brochure

Avoid weak generic CTAs when a stronger B2B action makes more sense.

## FAQ Topic Pool

List FAQ topics, not full answers.

They should match likely objections, buying questions, comparison questions, or informational follow-ups.

For commercial pages, most FAQ topics should help the reader evaluate fit, options, and next steps.

## Page Templates by Mode

### 1. Product Page

Typical structure:

- hero with positioning
- quick qualification block
- overview or use-case fit
- working principle or operating logic
- applications
- key specifications or parameter snapshot
- options or customization
- selection guidance
- concise trust block
- FAQ
- CTA

Use when the keyword points to one defined product or service.

### 2. Product Collection Page

Typical structure:

- hero introducing the product family
- family overview
- subtype comparison
- module for each major subtype
- use cases
- selection guidance
- technical overview or comparison block
- FAQ
- CTA

If the brief includes multiple machine types or variants, break them into separate subtype modules.

### 3. Category Page

Typical structure:

- hero for the broader category
- category overview
- main solution groups
- featured subcategories or products
- industry or use-case paths
- buying guidance
- FAQ
- CTA

Use when the keyword is broader than one family but still commercial.

### 4. Blog Article

Typical structure:

- intro aligned with the query
- direct answer or problem framing
- core explanation sections
- comparison or process section when relevant
- practical considerations
- soft trust block
- FAQ
- soft CTA

Use when the user mainly wants information or guidance, but the article should still move toward decision support.

### 5. Landing Page

Typical structure:

- strong hero for the specific audience or use case
- problem framing
- solution recommendation
- supporting products or services
- benefits and proof points
- process or implementation summary
- FAQ
- strong CTA

Use when conversion intent is tied to an industry, application, audience segment, or campaign.

## Collection Page Rule

If the page type is `Product collection page`, always do these extra steps:

1. Identify the major subtypes from the brief
2. Create one module for each subtype
3. Suggest whether each subtype deserves its own child page
4. Add internal link suggestions from the collection page to those child pages

If the user mentions examples such as `Single Shaft`, `Double Shaft`, `Automatic`, or `Portable`, treat them as required subtype modules when relevant.

## Notes for Writers

Use this section to tell downstream writers how to execute the page.

Examples:

- which sections deserve the most detail
- which sections should stay concise
- where structured evidence is mandatory
- where commercial intent should be strongest
- where brand mention should stay brief
- whether the tone should feel technical, consultative, practical, or comparison-led
- whether the brand should be handled under a stricter corporate-safe standard

## Guardrails

- Do not invent technical specs, certifications, or performance claims
- Do not build page plans that rely on vague self-promotional company copy to carry the page
- Do not encourage brand sections that would be risky, weakly sourced, or overly promotional for a listed company
- Do not ignore clear topic-evidence mismatch; flag it in `Evidence Alignment Check`
- Do not force every keyword into headings
- Do not recommend a page structure that conflicts with the inferred search intent
- Do not output full-body copy
- Keep the architecture realistic for a business website
- Prefer commercial clarity over SEO theater
- Do not output a URL unless the user explicitly requests one
- Do not plan H2 sections that expose SEO strategy to the reader, such as sections about related search terms, keyword overlap, or search intent differences. These belong in `Internal Link Suggestions` or `Notes for Writers`

## Handoff

The output should be ready for the next step:

- section-by-section drafting
- writer assignment
- page design planning
- CMS publishing setup
