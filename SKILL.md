---
name: seo-page-architect
description: Generate an SEO page architecture from a keyword brief for the United States English market. Use when the user wants a page topic, title, meta description, keyword set, H1-H3 structure, page module order, internal linking suggestions, CTA suggestions, FAQ topic pool, and page-type-specific architecture for product pages, product collection pages, category pages, blog articles, or landing pages.
---

# SEO Page Architect

Use this skill when the user already has a keyword brief and needs a page plan that can be handed to a writer, designer, SEO lead, or content manager.

This skill is for page architecture, not full copywriting.

## Default Market

Unless the user explicitly overrides it, assume:

- Target country: United States
- Target language: English

## Purpose

Convert a keyword brief into a page structure that matches search intent and business goals.

The output must be practical and publishing-oriented, not theoretical.

## Expected Inputs

Preferred input:

- A keyword brief generated from upstream research

The brief should ideally include:

- Primary keyword
- Secondary keywords
- Long-tail keywords
- Search intent
- Recommended page type
- Topic angles
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

If some fields are missing, infer carefully from the available brief. Do not invent specific product facts.

## Role

Your job is to:

1. Read the keyword brief
2. Confirm the best page pattern for the intent
3. Build an SEO-friendly page structure
4. Keep the page aligned with likely user intent
5. Prepare a plan suitable for downstream writing and publishing

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

- Product page: use for a specific machine, model, or tightly defined commercial term
- Product collection page: use for a broad product family with multiple machine types or variants
- Category page: use for a broader catalog or grouped solution area
- Blog article: use for informational or educational intent
- Landing page: use for campaign-like, industry-specific, use-case-specific, or conversion-focused intent

For B2B industrial keywords:

- model-specific or equipment-specific terms often fit product pages
- broad equipment family terms often fit collection pages
- industry application terms may fit landing pages or category pages
- question-based and educational terms usually fit blog articles

## Output Requirements

Always output in this structure.

Keep it compact, practical, and ready for downstream writing.

```markdown
Page Topic

Title

Description

Keywords

H1

## H2-H3 Structure
### H2:
- H3:

## Page Module Order
1.

## Internal Link Suggestions
- 

## CTA Suggestions
- 

## FAQ Topic Pool
- 

## Notes for Writers
- 
```

The opening block should follow this style:

```markdown
Waste Bag Opener Machine

Title
Waste Bag Opener Machine for Waste Sorting | Single & Double Shaft Solutions

Description
Efficient waste bag opener machines for MSW sorting plants. Explore single shaft and double shaft bag openers for high throughput, reduced material damage, and optimized waste separation.

Keywords
bag opener machine, waste bag opener, MSW bag opener, single shaft bag opener, double shaft bag opener, garbage bag breaking machine, waste sorting equipment, bag opener for recycling plant
```

Do not output a URL unless the user explicitly asks for one.

If the page type is `Product collection page`, also include:

```markdown
## Product Subtype Modules
- Subtype:
  Purpose:
  Suggested placement:

## Future Child Pages
- 
```

## Output Standards

### Page Topic

- Use the main page subject or primary keyword as the heading of the output
- Keep it concise
- Use title case when natural for English SEO deliverables

### Title

- Must align closely with the primary keyword
- Must reflect the page type and likely search intent
- Prefer clarity over cleverness
- Avoid obvious keyword stuffing

### Description

- Write for click-through, not just keyword repetition
- Keep it natural and commercially useful
- Mention product value, use case, or selection angle when relevant

### Keywords

- Output a comma-separated keyword set
- Include the primary keyword first
- Follow with closely related secondary keywords
- Use only terms supported by the brief
- Do not stuff weak or barely related phrases

### H1-H3 Structure

- Organize sections by user decision flow
- Avoid repetitive headings that restate the same keyword
- Use secondary and long-tail keywords naturally
- Make the structure suitable for a 1500-2000 word page when expanded

### Page Module Order

List the page blocks in publishing order.

Examples depending on page type:

- hero section
- key benefits
- product overview
- subtype selector
- applications
- technical parameters
- comparison table
- FAQ
- CTA

### Internal Link Suggestions

Recommend realistic internal links such as:

- related product pages
- subtype pages
- application pages
- FAQ pages
- blog guides
- contact page
- quote request page

These should support topic depth and conversion flow.

### CTA Suggestions

Recommend CTA language that fits the page type:

- Request a Quote
- Talk to an Engineer
- Download Brochure
- Compare Models
- Get Pricing
- Ask About Customization

Avoid generic CTAs if a stronger B2B action makes more sense.

### FAQ Topic Pool

List FAQ topics, not full answers.

They should match likely objections, buying questions, comparison questions, or informational follow-ups.

## Page Templates by Mode

### 1. Product Page

Typical structure:

- Hero with product positioning
- Core features
- Working principle or process
- Applications
- Technical specifications
- Optional configurations
- Why choose this machine
- FAQ
- CTA

Use when the keyword points to one defined machine or one product type.

### 2. Product Collection Page

Typical structure:

- Hero introducing the product family
- Product family overview
- Subtype comparison
- Module for each major subtype
- Use cases
- Selection guidance
- Technical overview or comparison table
- FAQ
- CTA

If the brief includes multiple machine types, break them into separate subtype modules.

Also suggest future child pages for each subtype when appropriate.

### 3. Category Page

Typical structure:

- Hero for the broader category
- Category overview
- Main solution groups
- Featured products
- Industry or use-case paths
- Buying guidance
- FAQ
- CTA

Use when the keyword is broader than one product family but still commercial.

### 4. Blog Article

Typical structure:

- Intro aligned with the query
- Core explanation sections
- Comparison or process section
- Practical considerations
- FAQ
- Soft CTA

Use when the user mainly wants information, explanation, or guidance.

### 5. Landing Page

Typical structure:

- Strong hero for the specific audience or use case
- Pain points
- Solution framing
- Relevant products or services
- Benefits and proof points
- FAQ
- Strong CTA

Use when conversion intent is tied to an industry, campaign, use case, or audience segment.

## Collection Page Rule

If the page type is `Product collection page`, always do these extra steps:

1. Identify the major subtypes from the brief
2. Create one module for each subtype
3. Suggest whether each subtype deserves its own child page
4. Add internal link suggestions from the collection page to those child pages

If the user mentions examples such as `Double Shaft` and `Single Shaft`, treat them as required subtype modules.

For collection pages, the title, description, keywords, H1, and section structure should reflect the broader product family first, then support each subtype clearly underneath.

## Notes for Writers

Use this section to tell downstream writers how to execute the page, for example:

- which sections deserve the most detail
- which sections should stay concise
- which supporting keywords should be distributed into headings
- where commercial intent should be strongest
- whether the tone should feel technical, consultative, or educational

## Guardrails

- Do not invent technical specs, certifications, or performance claims
- Do not force every keyword into headings
- Do not recommend a page structure that conflicts with the inferred search intent
- Do not output full-body copy
- Keep the architecture realistic for a business website
- Prefer commercial clarity over SEO theater
- Do not output a URL unless the user explicitly requests one

## Handoff

The output should be ready for the next step:

- section-by-section content drafting
- writer assignment
- page design planning
- CMS publishing setup
