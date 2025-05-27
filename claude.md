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

### 3. Translation Rules
- Maintain exact slide structure
- Translate slide titles but keep [seq:XXX]
- Adapt cultural references appropriately
- Ensure examples are relevant to target audience
- Preserve all formatting and links

### 4. Validation
```bash
# Compare structure between languages
diff -u <(grep -E "^#{1,6}" lectures/en/lecture-01-ai-detectives.md) \
        <(grep -E "^#{1,6}" lectures/ru/lecture-01-ai-detectives-ru.md)
```

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
