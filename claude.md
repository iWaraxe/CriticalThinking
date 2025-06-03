# Critical Thinking in the Age of AI - Course Development Guide

## Course Structure Requirements

### Slide Format Rules
1. **Each slide (##### level) must contain NO MORE THAN ONE of each section type:**
   - One `###### SCRIPT` section
   - One `###### VISUAL` section  
   - One `###### NOTES` section
   - One `###### LINKS` section (optional)
   - One `###### DEMONSTRATION` section (optional)
   - One `###### ACTIVITY` section (optional)
   - One `###### REFLECTION` section (optional)
   - One `###### ARCHIVE` section (optional)

2. **Slide boundaries are marked by:**
   - Next slide header (`##### [seq:XXX]`)
   - OR section divider (`---`)

### Course Hierarchy
```
# Critical Thinking in the Age of AI
## Lecture X: Title
### X.X. Section (optional)
#### X.X.X Topic (optional)
##### [seq:XXX] Slide title
###### SCRIPT
###### VISUAL
###### NOTES
###### LINKS (optional)
###### DEMONSTRATION (optional)
###### ACTIVITY (optional)
###### REFLECTION (optional)
###### ARCHIVE (optional)
---
```

### Slide Structure Components
- **SCRIPT**: Conversational narrative (1-2 minutes speaking time)
- **VISUAL**: Slide design description with engagement elements
- **NOTES**: Discussion prompts, fun facts, real-world connections (text only)
- **LINKS**: Relevant URLs and references from source materials
- **DEMONSTRATION**: Interactive AI experiments with expected outcomes
- **ACTIVITY**: Hands-on student exercises or games
- **REFLECTION**: Critical thinking questions for deeper analysis
- **ARCHIVE**: Removed content with deletion rationale and date

## Course Creation Workflow

### Phase 1: Repository Analysis
```bash
# Check existing lecture files
ls lectures/en/
# Identify missing lectures based on syllabus
```

### Phase 2: File Creation
Create missing lecture files following naming convention:
```
lecture-01-ai-detectives.md
lecture-02-how-ai-thinks.md
lecture-03-bias-detectives.md
lecture-04-error-alert.md
lecture-05-question-masters.md
lecture-06-ai-ethics-arena.md
lecture-07-creative-lab.md
lecture-08-showcase-launch.md
```

### Phase 3: Structure Planning
For each lecture, analyze the syllabus and create hierarchical structure:
1. Review lecture objectives and key topics
2. Identify logical sections (3-4 per lecture)
3. Break down into topics if needed
4. Plan slide sequence (15-20 slides per lecture)

Example structure:
```markdown
## Lecture 1: AI Detectives - What's Real in Our Digital World?

### 1.1. Welcome to the AI Age
##### [seq:010] Course Introduction
##### [seq:020] Meet Your AI Neighbors

### 1.2. What is Critical Thinking?
##### [seq:030] Thinking Like a Detective
##### [seq:040] Questions Are Your Superpower
```

### Phase 4: Content Development
For each slide, develop content in this order:

1. **SCRIPT** - Write engaging narrative
   - Age-appropriate language (12-15 years)
   - Pop culture references
   - Interactive tone ("Let's explore...", "Can you imagine...")

2. **VISUAL** - Design slide elements
   - Main visual concept
   - Text overlays
   - Interactive elements
   - Color/style suggestions

3. **NOTES** - Add enrichment (text only)
   - Fun facts
   - Discussion starters
   - Common misconceptions
   - Real-world connections

4. **LINKS** - Reference materials
   - URLs from source materials
   - Relevant articles and studies
   - Tool documentation
   - Additional resources

5. **DEMONSTRATION** - Create AI interactions
   - Specific prompts to try
   - Expected vs actual results
   - What to observe
   - Follow-up experiments

### Phase 5: Quality Checks
- Verify each slide has required sections
- Check narrative flow between slides
- Ensure activities are age-appropriate
- Validate AI demonstrations work as intended

## Translation Workflow

### 1. Monitor English Updates
```bash
# Check for changes in English files
git diff lectures/en/
```

### 2. Translation Process
When English file is updated:
1. Identify changed sections using git diff
2. Load both English and target language files
3. Translate only updated content
4. Preserve structure and seq numbers
5. Keep section headers (SCRIPT, VISUAL, etc.) in English

### 3. Translation and Localization Rules
- Maintain exact slide structure
- Translate slide titles but keep [seq:XXX]
- **CRITICAL**: Apply deep cultural localization (see Localization Guidelines below)
- Ensure examples are relevant to target audience
- Preserve all formatting and links
- Replace generic examples with locally relevant ones
- Use appropriate local slang and expressions for teenagers
- Reference local institutions, celebrities, and cultural phenomena

### 4. Validation
```bash
# Compare structure between languages
diff -u <(grep -E "^#{1,6}" lectures/en/lecture-01-ai-detectives.md) \
        <(grep -E "^#{1,6}" lectures/ru/lecture-01-ai-detectives-ru.md)
```

## Comprehensive Localization Guidelines

### Target Countries and Cultural Context
The course serves company offices in: Belarus, Lithuania, Poland, Romania, Ukraine, Bulgaria, Moldova, Georgia, and Mexico. Each translation should reflect local culture while maintaining universal appeal.

### Core Localization Principles

#### 1. Cultural References and Examples
**Replace generic examples with locally relevant ones:**

**Technology Examples:**
- Popular local apps and platforms
- Local tech companies and startups
- Regional social media trends
- Country-specific digital services

**Pop Culture References:**
- Local musicians, YouTubers, influencers popular with teens
- National TV shows, movies, memes
- Local gaming communities and streamers
- Regional sports heroes and celebrities

**Historical and Educational Context:**
- Local historical events for timeline examples
- National heroes and figures for inspiration
- Local educational system references
- Regional scientific achievements

#### 2. Institutional and Authority References

**Government and Official Sources:**
- National statistical offices (.gov domains)
- Educational ministries and agencies
- Local universities and research institutions
- National tech/digital initiatives

**Verification Sources:**
- Trusted local news outlets
- Fact-checking organizations in local language
- Regional academic institutions
- Local tech community resources

#### 3. Language and Communication Style

**Age-Appropriate Local Slang:**
- Research current teenage slang and expressions
- Use natural, conversational tone for the region
- Include popular local expressions and idioms
- Avoid outdated or formal language

**Cultural Communication Patterns:**
- Adapt humor style to local preferences
- Consider cultural attitudes toward authority/questioning
- Respect local educational traditions while encouraging critical thinking
- Use familiar metaphors and analogies

#### 4. Economic and Social Context

**Local Issues and Challenges:**
- Regional digital divide considerations
- Local privacy/surveillance concerns
- Economic realities (free vs paid tools)
- Regional internet infrastructure limitations

**Relevant Local Problems:**
- Country-specific misinformation challenges
- Local bias examples in AI systems
- Regional ethical considerations
- Local regulatory environment

### Country-Specific Localization Guidance

#### 🇺🇦 Ukraine (Lviv Office)
**Cultural Elements:**
- Ukrainian tech sector with Lviv focus (SoftServe, EPAM Lviv, Intellias)
- Popular Ukrainian YouTubers and regional Lviv influencers
- Ukrainian traditional elements (vyshyvanka, bandura) mixed with Galician culture
- References to Ukrainian resilience and Western Ukrainian innovation
- Lviv-specific landmarks (Rynok Square, Freedom Avenue, Opera Theatre)
- Local educational institutions (Lviv Polytechnic, LNU named after Ivan Franko)

**Language Considerations:**
- Use contemporary Ukrainian with subtle Galician influence
- Include modern Ukrainian slang popular with Lviv teens
- Reference local Telegram channels and social media groups
- Mention local media outlets (Zaxid.net, Varta1, LvivNow)

**Local Context:**
- Digital literacy as empowerment tool during wartime
- Importance of fact-checking during information warfare
- Lviv as Western Ukrainian tech hub
- Local cybersecurity awareness and European integration
- Coffee culture and startup ecosystem references
- Historical context of Lviv as cultural/educational center

#### 🇧🇾 Belarus
**Cultural Elements:**
- Belarusian IT sector (Epam, Wargaming)
- Local tech community and High Tech Park
- Traditional Belarusian culture mixed with modern tech
- Regional gaming and esports scene

**Local Context:**
- Strong IT education tradition
- Tech as economic opportunity
- Digital privacy and security awareness
- Innovation within constraints

#### 🇱🇹 Lithuania
**Cultural Elements:**
- Baltic tech scene and Fintech sector
- Lithuanian gaming industry (Nordcurrent)
- Baltic cooperation and European integration
- Local startup ecosystem

**Local Context:**
- Digital government initiatives
- European GDPR framework
- Baltic cybersecurity cooperation
- Innovation in small nations

#### 🇵🇱 Poland
**Cultural Elements:**
- Polish gaming industry (CD Projekt, Techland)
- Popular Polish YouTubers and influencers
- Polish tech companies and startups
- Traditional Polish culture in digital age

**Local Context:**
- Strong gaming culture among teens
- European digital rights framework
- Polish digital transformation initiatives
- Regional tech leadership

#### 🇷🇴 Romania
**Cultural Elements:**
- Romanian tech sector and outsourcing industry
- Local gaming and esports community
- Romanian tech education programs
- Bucharest tech scene

**Local Context:**
- Growing tech sector opportunities
- European digital framework
- Regional digital transformation
- Innovation hubs and tech parks

#### 🇧🇬 Bulgaria
**Cultural Elements:**
- Bulgarian tech and outsourcing sector
- Local gaming and software development
- Sofia tech ecosystem
- Bulgarian contributions to global tech

**Local Context:**
- Tech education and career opportunities
- European digital rights
- Regional innovation initiatives
- Balkan tech cooperation

#### 🇲🇩 Moldova
**Cultural Elements:**
- Moldovan tech sector development
- Regional tech education initiatives
- Chisinau tech community
- Cross-border tech cooperation

**Local Context:**
- Emerging tech opportunities
- Digital transformation goals
- Tech as development pathway
- Regional collaboration

#### 🇬🇪 Georgia
**Cultural Elements:**
- Georgian tech sector and innovation
- Tbilisi tech scene
- Georgian startup ecosystem
- Traditional culture meets innovation

**Local Context:**
- Government digitalization efforts
- Tech as economic diversification
- Regional tech cooperation
- Innovation in post-Soviet context

#### 🇲🇽 Mexico
**Cultural Elements:**
- Mexican tech ecosystem (Clip, Kavak, Bitso)
- Popular Mexican YouTubers, streamers, and influencers
- Traditional Mexican culture (alebrije, Día de Muertos, lucha libre) in creative examples
- Mexican music scene (reggaetón, mariachi fusion, regional Mexican)
- Local gaming and esports community

**Language Considerations:**
- Use contemporary Mexican Spanish with natural teen slang
- Include popular Mexican expressions and modismos
- Reference Mexican social media platforms and trends
- Avoid overly formal or Spain Spanish terminology

**Local Context:**
- Growing fintech and startup ecosystem
- Digital transformation in education and government
- STEM education initiatives and opportunities
- Mexican innovation in Latin American context
- Digital divide and accessibility considerations
- Local regulatory environment (INAI, IFT)

**Educational and Cultural References:**
- Mexican educational system (SEP, preparatoria, universidad)
- Local universities and tech programs (Tec de Monterrey, UNAM)
- Mexican scientific achievements and innovators
- Regional variations and cultural diversity within Mexico
- Mexican-American tech connections and opportunities

### Implementation Checklist for Each Localization

#### Content Adaptation:
- [ ] Replace 5+ generic examples with local ones per lecture
- [ ] Include 3+ local cultural references per lecture
- [ ] Reference local institutions and authorities
- [ ] Use age-appropriate local slang and expressions
- [ ] Adapt humor and communication style

#### Technical Adaptation:
- [ ] Verify AI tools availability/accessibility in region
- [ ] Provide local alternatives where needed
- [ ] Reference local regulations and privacy laws
- [ ] Include local tech career pathways

#### Cultural Sensitivity:
- [ ] Review content with native speaker familiar with teen culture
- [ ] Ensure examples respect local values and traditions
- [ ] Avoid potential political sensitivities
- [ ] Balance global perspective with local relevance

#### Quality Assurance:
- [ ] Test all local examples and references for accuracy
- [ ] Verify local institutions and websites are current
- [ ] Confirm cultural references are appropriate and current
- [ ] Validate language is natural and engaging for teens

### Localization Resources by Country

#### Research Sources:
- Local teenage social media trends and influencers
- National education ministry websites
- Local tech industry reports and news
- Regional youth culture studies and surveys
- Local fact-checking and media literacy organizations

#### Collaboration Partners:
- Local tech communities and educators
- Regional AI and digital literacy initiatives
- Youth organizations and programs
- Local tech companies and startups

## Content Guidelines

### Tone and Style
- **Playful**: Use games, challenges, detective metaphors
- **Inclusive**: Examples from diverse backgrounds
- **Empowering**: "You can..." rather than "You should..."
- **Question-driven**: Encourage curiosity

### AI Tools Integration
Primary tools for demonstrations:
- ChatGPT, Claude (text generation)
- Midjourney, DALL-E (images)
- Perplexity (research)
- HeyGen (avatars)

### Activity Types
1. **Detective Challenges**: Spot AI errors/bias
2. **Creation Labs**: Make something with AI
3. **Debate Arenas**: Ethical discussions
4. **Fact-Check Races**: Verify information
5. **Role-Play Scenarios**: Act out AI dilemmas

## Course Update Workflow - Keeping Content Current

### Overview
This workflow ensures the course stays relevant with the latest AI developments while maintaining quality and preventing content bloat. Updates should be strategic, replacing outdated content rather than just adding new material.

### 1. Receiving Update Materials
When user provides new AI developments:
- News articles and press releases
- YouTube video transcripts
- Research papers and studies
- Product announcements
- Ethical controversies or incidents
- New AI tools or capabilities

### 2. Version Control Process
```bash
# Create feature branch for updates
git checkout -b update/ai-news-YYYY-MM-DD

# Work on updates
# Commit changes with descriptive messages
git add -A
git commit -m "Update: [Brief description of changes]"

# Push branch for review
git push -u origin update/ai-news-YYYY-MM-DD
```

### 3. Content Analysis Strategy

#### Step 1: Categorize New Information
Analyze incoming materials and categorize by:
- **Technology Updates**: New models, capabilities, tools
- **Bias/Ethics Cases**: New examples of AI bias or ethical dilemmas
- **Failures/Errors**: Recent AI mistakes or limitations
- **Success Stories**: Positive AI applications
- **Regulatory Changes**: New laws or guidelines
- **Cultural Shifts**: Changes in how society views/uses AI

#### Step 2: Map to Existing Content
Identify where updates belong:
- New AI models → Lecture 2 (How AI Thinks)
- Bias examples → Lecture 3 (Bias Detectives)
- Error cases → Lecture 4 (Error Alert!)
- Ethical dilemmas → Lecture 6 (AI Ethics Arena)
- Creative tools → Lecture 7 (AI Creative Lab)
- Future trends → Lecture 8 (Future Showcase)

#### Step 3: Evaluate Current Content
For each affected section:
1. **Identify outdated content**
   - Old AI models no longer relevant
   - Resolved controversies
   - Superseded technologies
   - Outdated statistics or claims

2. **Assess content balance**
   - Is this section getting too long?
   - Are examples still diverse and engaging?
   - Does it maintain age-appropriate complexity?

### 4. Update Implementation Guidelines

#### Content Replacement Strategy
**DO:**
- Replace outdated examples with new ones
- Update statistics and facts
- Refresh pop culture references
- Modernize demonstrations
- Streamline verbose sections
- Move removed content to ARCHIVE section
- Add URLs to LINKS section
- Keep NOTES text-only

**DON'T:**
- Just append new content to existing
- Delete information permanently (use ARCHIVE)
- Let any lecture exceed 60 minutes
- Add complexity beyond age level
- Create new sections without removing old
- Put links in NOTES (use LINKS section)

#### Update Priorities
1. **High Priority** (Update immediately):
   - Factual errors or outdated information
   - Broken demonstrations
   - Deprecated AI tools
   - Resolved controversies presented as current

2. **Medium Priority** (Update within month):
   - Better examples available
   - More relevant local references
   - Improved demonstrations
   - Clearer explanations

3. **Low Priority** (Consider in quarterly review):
   - Minor terminology changes
   - Aesthetic improvements
   - Additional resources

### 5. Practical Update Examples

#### Example 1: New AI Model Released
**Material**: "GPT-5 released with video understanding"
**Action**: 
- Update Lecture 2, slide [seq:040] "How AI Models Work"
- Replace GPT-3 examples with GPT-5
- Add video understanding to capabilities
- Move GPT-3 content to ARCHIVE with rationale
- Add source URL to LINKS section

#### Example 2: Major AI Bias Incident
**Material**: "AI hiring tool discriminates against women"
**Action**:
- Update Lecture 3, slide [seq:060] "Real-World Bias"
- Replace older example with this current one
- Update DEMONSTRATION with new bias detection exercise
- Move old example to ARCHIVE with explanation
- Add article URL to LINKS section

#### Example 3: New Creative AI Tool
**Material**: "Sora creates realistic videos from text"
**Action**:
- Update Lecture 7 demonstrations
- Replace older video tool example
- Add new creative activity using Sora
- Archive old tool information with deprecation note
- Add Sora documentation link to LINKS section

### 6. Quality Assurance Checklist

Before finalizing updates:
- [ ] Each lecture still fits 60-minute timeframe
- [ ] Examples are balanced (not all negative/positive)
- [ ] Content remains age-appropriate
- [ ] Local cultural references still relevant
- [ ] Demonstrations tested and working
- [ ] No redundant information across lectures
- [ ] Clear improvement over previous version
- [ ] All languages updated consistently

### 7. Update Documentation

After updates, document changes:
```markdown
## Update Log: YYYY-MM-DD

### Materials Reviewed:
- [List of articles/sources provided]

### Changes Made:
- Lecture 2: Updated AI model examples (seq:040, seq:050)
- Lecture 3: Replaced bias case study (seq:060)
- Lecture 7: New creative tool demonstration

### Content Removed:
- Outdated GPT-3 examples
- 2022 bias incident (resolved)
- Deprecated tool references

### Rationale:
[Brief explanation of why these changes improve the course]
```

### 8. Language Version Management
**IMPORTANT**: Updates are made ONLY to English version. Other language versions are updated separately when course delivery is ordered for specific countries.

Process:
1. All updates go to English lectures only
2. Document which slides/sections were updated
3. When course is ordered for specific country:
   - User will manually transfer changes to target language
   - Apply cultural localization during transfer
   - Ensure demonstrations work in target region

## Lecture Development Checklist

For each lecture:
- [ ] File created with correct naming
- [ ] Structure planned (sections/topics)
- [ ] All slides have seq numbers
- [ ] Each slide has SCRIPT section
- [ ] Each slide has VISUAL section
- [ ] Each slide has NOTES section (text only)
- [ ] LINKS section added where relevant
- [ ] Key slides have DEMONSTRATION
- [ ] ARCHIVE section used for removed content
- [ ] Activities distributed throughout
- [ ] Homework assignment included
- [ ] Resources listed at end

## Common Integration Points

### By Topic:
- **AI Basics** → Lecture 1, seq:020-050
- **How AI Works** → Lecture 2, entire lecture
- **Bias Examples** → Lecture 3, seq:040-080
- **Error Types** → Lecture 4, seq:030-070
- **Prompting Tips** → Lecture 5, seq:040-090
- **Ethics Dilemmas** → Lecture 6, seq:050-100
- **Creative Tools** → Lecture 7, demonstrations
- **Future Thinking** → Lecture 8, seq:020-060

### Cross-Cutting Themes:
- **Critical Questions** → Every lecture intro
- **Fact-Checking** → Lectures 2, 4, 5
- **Ethics** → Woven throughout, focus in 6
- **Creativity** → Lectures 1, 7, 8
- **Real-World Impact** → All lecture conclusions

## Important Notes

- Each lecture = 60 minutes of content
- Include 10-minute break in timing
- Balance screen time with discussions
- Test all AI demonstrations before class
- Have offline alternatives ready
- Encourage experimentation over perfection
- Celebrate "productive failures"

## Success Metrics

Well-developed lecture includes:
- Clear learning objectives met
- 3-4 interactive activities
- 2-3 AI demonstrations
- 1 creative challenge
- Multiple discussion prompts
- Homework that reinforces concepts
- Resources for further exploration
