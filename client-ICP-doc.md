# Client ICP Documentation Skill

**Skill name:** `/client-ICP-doc`

**Purpose:** Extract, structure, and document Ideal Customer Profile (ICP) data for client projects, creating ready-to-use deliverables including company lists, contact lists, and strategic documentation.

---

## When to Use This Skill

Use this skill when you need to:
- Create or update client ICP documentation from research
- Structure company and contact data into standardized CSV formats
- Build strategic case studies or pitch documents with ICP data
- Validate and correct ICP documentation for accuracy
- Prepare ICP deliverables for client review

---

## Core ICP Data Structure

### Company Data Format (companies.csv)

**Required columns:**
```
Name,Domain,Description,Industry,Size,Type,City,State or Province,Country,Company LinkedIn URL,Company Fit,Reason
```

**Company Fit ratings:**
- `GREAT` - Strong operational fit, documented support processes, high alignment
- `GOOD` - Solid fit with relevant operations, clear service needs
- `MODERATE` - Basic fit, some alignment with services

**Reason format:**
```
[Company] [brief operational description]. [Specific evidence of service needs]. [Why relevant to client's capabilities].

Best outreach angle: [Specific service areas]
```

**Rules:**
- Use official company descriptions from LinkedIn or company websites
- Cite specific evidence (official websites, documented processes, published data)
- Avoid speculation - only document verifiable information
- Include employee count ranges, not exact numbers unless official
- State facts, not assumptions about purchasing intent

### Contact Data Format (leads.csv)

**Required columns:**
```
First Name,Last Name,Title,Company,Domain,Email,Phone,LinkedIn URL,Signals,Source,Research Date,Qualification Score
```

**Email verification:**
- Mark verified emails as `EMAIL VERIFIED` in display (not in CSV)
- Include verification explanation in documentation
- Never claim an email is verified without actual verification

**Qualification scores:**
- Document assessment criteria clearly
- Explain scoring methodology
- Never claim scores are "calculated" - say "assessed" or "documented"

---

## Documentation Standards

### Writing Style

**Always use first-person ("I" not "we"):**
- ✅ "I've identified 9 qualified companies..."
- ❌ "We've identified 9 qualified companies..."

**Mark proposed/suggested items clearly:**
- ✅ "Proposed Month 1 Industry Allocation"
- ❌ "Month 1 Industry Allocation" (sounds confirmed)

**Avoid claiming confirmed intent:**
- ✅ "These signals may suggest a need for support"
- ❌ "These signals confirm they need support"

**Use specific, verifiable language:**
- ✅ "According to its official website..."
- ✅ "Its published case study reports..."
- ❌ "They probably need..."
- ❌ "It's likely that..."

### Protecting Proprietary Information

**Never reveal specific tools:**
- ✅ "I use established B2B research platforms"
- ❌ "I use Apollo, Clay, and ZoomInfo"

**Generic capability descriptions:**
- ✅ "Data enrichment platforms"
- ✅ "Email verification services"
- ✅ "CRM and outreach tools"
- ❌ "Salesforce Service Cloud"
- ❌ "Zendesk"
- ❌ "Loom"

---

## Common Corrections Checklist

When reviewing or correcting ICP documentation:

**1. Company Data Accuracy**
- [ ] Verify employee counts match official sources
- [ ] Confirm operational facts (store counts, geographic reach, etc.)
- [ ] Remove specific hours/times unless critical
- [ ] Update any outdated information
- [ ] Check all company descriptions for accuracy

**2. Contact Data Quality**
- [ ] Remove duplicate contacts
- [ ] Verify email addresses are current
- [ ] Update job titles if changed
- [ ] Remove outdated contacts
- [ ] Update contact counts automatically

**3. Language and Tone**
- [ ] All writing is first-person ("I" not "we")
- [ ] Proposed/suggested items marked clearly
- [ ] No claims of confirmed purchasing intent
- [ ] No speculation presented as fact
- [ ] Specific tool names removed

**4. Verification and Proof**
- [ ] "VERIFIED" changed to "EMAIL VERIFIED" where applicable
- [ ] Verification explanation included
- [ ] All claims cite sources
- [ ] Assessment criteria explained
- [ ] Avoid "calculated scores" language

**5. Strategic Positioning**
- [ ] ICP allocations marked as "proposed"
- [ ] Qualification criteria clearly stated
- [ ] Market signals described with appropriate hedging
- [ ] Outreach intent clearly separated from confirmed interest

---

## Standard Deliverables

### 1. Company List (companies.csv)
- 9-15 qualified companies
- Complete company profiles
- Fit assessments with reasoning
- Best outreach angles

### 2. Contact List (leads.csv)
- 15-25 decision-maker contacts
- Complete contact information
- Qualification assessments
- Research documentation

### 3. Strategic Documentation
- ICP overview and targeting criteria
- Industry allocation (marked as proposed)
- Market signals and research methodology
- Sample outreach messaging
- 30-day execution plan

---

## File Locations

**Standard project structure:**
```
/project-name/
├── index.html (if dashboard/presentation)
├── companies.csv
├── leads.csv
└── README.md (optional)
```

**GitHub repository:**
- Always push to appropriate GitHub repository
- Commit with clear, descriptive messages
- Include what changed and why

---

## Quality Standards

**Before finalizing any ICP documentation:**

1. **Accuracy Check**
   - Every fact verified against official sources
   - No speculation or assumptions presented as fact
   - All numbers/figures match official data

2. **Consistency Check**
   - Writing style consistent throughout
   - First-person voice everywhere
   - Terminology consistent

3. **Completeness Check**
   - All required fields populated
   - Contact counts accurate
   - All references to counts updated

4. **Clarity Check**
   - Proposed items clearly marked
   - Assessment criteria explained
   - No ambiguous claims

5. **Professional Standards**
   - No proprietary tool names
   - No overpromising on results
   - Appropriate hedging on intent/signals

---

## Example: Correcting ICP Documentation

**Task:** "Update the company list with corrected information"

**Process:**
1. Read the current companies.csv
2. Identify what needs correction
3. Verify correct information from official sources
4. Update specific rows using Edit tool
5. Update all dependent counts in documentation
6. Commit and push changes with clear message

**Commit message format:**
```
Correct [specific item] in company data

- Changed [old value] to [new value]
- Source: [official source]
- Updated all dependent references
```

---

## Notes

- This skill focuses on ICP documentation quality and accuracy
- For full client onboarding, use `/client-onboarding-intelsol` skill
- For Clay filter generation, see position list rules in CLAUDE.md
- Always verify information before updating documentation
- When in doubt, cite sources and use appropriate hedging

---

**Last updated:** 2026-11-17
**Version:** 1.0
