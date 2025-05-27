# Critical Thinking in the Age of AI - Course Development Guide

## Course Structure Requirements

### Slide Format Rules
1. **Each slide (##### level) must contain NO MORE THAN ONE of each section type:**
   - One `###### SCRIPT` section
   - One `###### VISUAL` section  
   - One `###### NOTES` section
   - One `###### DEMONSTRATION` section (optional)
   - One `###### ACTIVITY` section (optional)
   - One `###### REFLECTION` section (optional)

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
###### DEMONSTRATION (optional)
###### ACTIVITY (optional)
###### REFLECTION (optional)
---
```

### Slide Structure Components
- **SCRIPT**: Conversational narrative (1-2 minutes speaking time)
- **VISUAL**: Slide design description with engagement elements
- **NOTES**: Discussion prompts, fun facts, real-world connections
- **DEMONSTRATION**: Interactive AI experiments with expected outcomes
- **ACTIVITY** (new optional): Hands-on student exercises or games
- **REFLECTION** (new optional): Critical thinking questions for deeper analysis

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

3. **NOTES** - Add enrichment
   - Fun facts
   - Discussion starters
   - Links to resources
   - Common misconceptions

4. **DEMONSTRATION** - Create AI interactions
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

#### 🇺🇦 Ukraine
**Cultural Elements:**
- Ukrainian tech sector (Ajax Systems, Grammarly)
- Popular Ukrainian YouTubers and influencers
- Ukrainian traditional elements (vyshyvanka, bandura) in creative examples
- References to Ukrainian resilience and innovation

**Language Considerations:**
- Use contemporary Ukrainian, not Soviet-era terminology
- Include modern Ukrainian slang popular with teens
- Reference Ukrainian social media platforms and trends

**Local Context:**
- Digital literacy as empowerment tool
- Importance of fact-checking during information warfare
- Ukrainian AI and tech initiatives
- Local cybersecurity awareness

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

## Update Workflow (Future)

### 1. Identify Update Location
Map new content to existing structure:
- New AI models → Lecture 2 (How AI Works)
- Bias examples → Lecture 3 (Bias Detection)
- Ethics cases → Lecture 6 (Ethics Arena)
- New tools → Relevant demonstration sections

### 2. Integration Strategy
- Enhance existing sections, don't duplicate
- Add to NOTES for minor updates
- Revise SCRIPT for major changes
- Update DEMONSTRATION with new examples

### 3. Version Control
```bash
git checkout -b update/description
# Make changes
git commit -m "Update: Add new AI capability to Lecture X"
```

## Lecture Development Checklist

For each lecture:
- [ ] File created with correct naming
- [ ] Structure planned (sections/topics)
- [ ] All slides have seq numbers
- [ ] Each slide has SCRIPT section
- [ ] Each slide has VISUAL section
- [ ] Each slide has NOTES section
- [ ] Key slides have DEMONSTRATION
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
