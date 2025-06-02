# Lecture 4: Error Alert! When AI Gets It Wrong

## 4.1. Welcome to Error Central!

### [seq:010] Previously on AI Detectives...

###### SCRIPT
Welcome back, detectives! We've learned how AI thinks and discovered its biases. Today, we're sounding the error alert! We'll explore the wild world of AI mistakes – from hilarious fails to dangerous errors. By the end, you'll be expert error spotters, ready to catch AI mistakes before they catch you!

###### VISUAL
- Error alert siren and warning lights theme
- Recap badges from previous lectures
- Error examples preview collage
- Students as "Error Response Team"

###### NOTES
- Start with funny errors to engage students
- Build to more serious implications
- Emphasize everyone makes mistakes - even AI

---

## 4.2. The Hall of Fame of AI Fails

### [seq:020] When AI Goes Hilariously Wrong

###### SCRIPT
Let's start with the fun stuff – AI fails that make us laugh! Like when AI told someone to put glue on pizza to keep cheese from sliding off, or when it suggested using gasoline to cook spaghetti faster. But here's a newer problem: Sometimes you think you're talking to one AI, but you're actually talking to a completely different one! Tools like Ollama have been caught calling a model "DeepSeek R1" when it's actually running a totally different model called "Qwen distill 8B." It's like ordering a pizza and getting tacos – confusing and potentially frustrating!

###### VISUAL
- Gallery of funny AI fails with reactions
- Screenshot examples of absurd suggestions
- NEW: Model name confusion examples (Ollama interface showing misleading names)
- "Common Sense: 0, Confidence: 100" meter
- Bait-and-switch visualization

###### NOTES
- These examples are real and documented
- Humor helps students remember the lesson
- Bridge from funny to "why this matters"
- NEW: Model naming crisis in 2025 with Ollama breaking open-source standards
- Users getting different AI than expected affects benchmarks and trust

###### ACTIVITY
"AI Fail Collection Enhanced":
1. Students share funny AI errors they've seen
2. NEW: Check what model they're actually using vs what the interface claims
3. Vote on "Most Ridiculous Fail" and "Most Confusing Model Name"
4. Analyze why AI made each mistake
5. Create class "Hall of Fame" display

---

## 4.3. Logic Errors: When 2+2=5

### [seq:030] AI's Math and Logic Meltdowns

###### SCRIPT
Here's something weird – AI can write beautiful poetry but sometimes fails at basic math! It might tell you that 2+2=5 with complete confidence, or claim that if all roses are flowers, then all flowers must be roses. These logic errors happen because AI learned patterns, not actual reasoning. It's like memorizing multiplication tables but not understanding what multiplication means!

###### VISUAL
- Math problems with wrong AI answers
- Logic puzzle failures illustrated
- Pattern matching vs actual calculation
- "Logic Error" warning signs

###### NOTES
- Emphasize difference between calculation and pattern matching
- AI often fails at simple tasks kids can do
- Importance of checking AI's work, especially in homework

###### DEMONSTRATION
"Stump the AI with Logic":
1. Give AI basic word problems
2. Try simple syllogisms
3. Ask for step-by-step math
4. Watch where it breaks down

---

## 4.4. The Deepfake Dilemma

### [seq:040] When Seeing Isn't Believing

###### SCRIPT
Now for something more serious – deepfakes. AI can now create videos of people saying things they never said, or photos of events that never happened. Imagine someone making a video of you saying something mean – but it's not really you! This technology is getting so good that our eyes can't tell the difference. Scary, right?

###### VISUAL
- Before/after showing deepfake creation
- Warning signs to spot deepfakes
- Real vs fake comparison
- "Trust but verify" message

###### NOTES
- Deepfakes used for entertainment and harm
- Political and personal implications
- Technology advancing faster than detection

###### ACTIVITY
"Deepfake Detective Training":
1. Show mix of real and deepfake videos
2. Students guess which is which
3. Reveal answers and discuss clues
4. Create detection checklist

---

## 4.5. Misinformation Multiplier

### [seq:050] How AI Spreads False Info

###### SCRIPT
Remember how AI learns from the internet? Well, the internet has lots of false information, and AI learned that too! It might confidently tell you about historical events that never happened, or spread conspiracy theories as facts. Even worse, people trust AI, so false info spreads faster. It's like a game of telephone on steroids!

###### VISUAL
- Misinformation spread diagram
- AI repeating false claims examples
- Trust cascade effect visualization
- Fact vs fiction balance scale

###### NOTES
- AI doesn't fact-check itself
- Confident tone makes lies believable
- Social media amplification effect

###### DEMONSTRATION
"Fact or Fiction Challenge":
1. AI generates mix of true/false statements
2. All sound equally confident
3. Students research to verify
4. Discuss danger of trusting blindly

---

## 4.6. The Overconfidence Problem

### [seq:060] Why AI Never Says "I Don't Know"

###### SCRIPT
Here's a huge problem – AI almost never admits when it doesn't know something. Ask it about a made-up book, and it'll write you a summary! Ask about a fake historical event, and it'll give you dates and details. But there's an even weirder problem: Some AI models completely ignore their instructions! DeepSeek R1, for example, struggles with "system prompts" – the behind-the-scenes instructions that tell it how to behave. It's like a student who confidently gives wrong answers AND doesn't follow the assignment instructions!

###### VISUAL
- Confidence meter stuck at maximum
- Examples of AI explaining nonexistent things
- NEW: System prompt failures illustration
- "I don't know" button that's never pressed
- Comparison with human uncertainty
- Instructions being ignored animation

###### NOTES
- AI designed to be helpful, not accurate
- No self-awareness of knowledge limits
- Confidence doesn't equal correctness
- NEW: DeepSeek R1 system prompt failures documented in May 2025
- Instructions need to go in user messages instead of system prompts
- Different models have different instruction-following capabilities

###### ACTIVITY
"Make AI Admit Ignorance & Follow Instructions":
1. Create increasingly obscure questions
2. See if AI ever says "I don't know"
3. NEW: Test if AI follows specific formatting instructions
4. Document confident wrong answers AND instruction failures
5. Compare different models' instruction-following abilities

---

## 4.7. Context Confusion

### [seq:070] When AI Misses the Point

###### SCRIPT
AI often misses context that humans understand instantly. Ask it about "running" and it might not know if you mean exercise, managing something, or a nose that's running! But here's something really concerning: AI performs differently based on what language you use! Recent tests show that DeepSeek R1 gives worse answers when forced to "think" in Russian or Finnish compared to English. This creates unfair advantages for English speakers and shows how AI can be accidentally biased against other languages and cultures!

###### VISUAL
- Same word, different contexts examples
- AI mixing up fictional and real contexts
- NEW: Language performance comparison chart
- Conversation going off the rails
- Context clues AI misses
- Global language bias illustration

###### NOTES
- Humans use tons of context AI can't access
- Sarcasm, humor, and metaphors confuse AI
- Cultural context often completely missed
- NEW: Multilingual reasoning performance varies significantly
- Chain-of-thought length correlates with answer quality regardless of language
- English-first training creates systematic disadvantages

###### DEMONSTRATION
"Context Chaos Enhanced":
1. Give AI ambiguous prompts
2. Watch it guess wrong context
3. Try sarcasm and metaphors
4. NEW: Test same question in different languages
5. Compare answer quality across languages
6. Discuss fairness implications

---

## 4.8. The Copy-Paste Problem

### [seq:080] When AI Plagiarizes

###### SCRIPT
Here's a sneaky error – sometimes AI doesn't create new text, it basically copy-pastes from its training! It might give you text that's too similar to existing work, getting you in trouble for plagiarism. Or it might repeat copyrighted content. It's not trying to cheat – it just learned patterns too well. Always make AI work your starting point, not your final answer!

###### VISUAL
- Side-by-side comparison of AI output and original
- Plagiarism detection software catching AI text
- "Inspired by" vs "Copied from" spectrum
- Student work process: AI draft → Human editing

###### NOTES
- Schools increasingly checking for AI plagiarism
- Legal issues with copyrighted content
- Importance of adding your own voice

###### ACTIVITY
"Originality Check":
1. Get AI to write about common topics
2. Search for similar sentences online
3. Find instances of near-copying
4. Practice proper AI attribution

---

## 4.9. Error Prevention Strategies

### [seq:090] Your Error-Catching Toolkit

###### SCRIPT
Now for the good news – you can catch these errors! Always fact-check important information. Look for logic that doesn't make sense. Question overconfident answers. Consider context. Check for originality. And most importantly, use your human brain! AI is a tool to help you think, not think for you. You're smarter than AI because you can actually understand!

###### VISUAL
- Error prevention checklist
- Verification workflow diagram
- Human + AI collaboration model
- "Error Shield" badge for students

###### NOTES
- Practical strategies students can use immediately
- Emphasize human judgment is irreplaceable
- Building good habits early

###### ACTIVITY
"Error Prevention Protocol":
1. Create class error-checking checklist
2. Practice on real AI outputs
3. Time trials: Quick checks that work
4. Make it a habit, not a chore

---

## 4.10. Homework & Next Time

### [seq:100] Mission: Error Hunter

###### SCRIPT
Your mission this week: Become an error hunter! Find different types of AI errors, document them, and practice our prevention strategies. Next week, we'll level up to become Question Masters – learning how to get the best possible answers from AI. Get ready to master the art of prompt engineering!

###### VISUAL
- Mission briefing style layout
- Error hunting checklist
- Preview of prompt engineering
- Resources and tools QR code

###### NOTES
- Encourage safe, responsible error hunting
- Remind about academic integrity
- Build excitement for prompt engineering

### Homework Assignment:
1. Collect 5 different types of AI errors
2. NEW: Check if the AI model you're using is actually what it claims to be
3. Test error prevention strategies
4. Create an "Error Alert" poster including model naming warnings
5. NEW: Test the same question in different languages (if you speak any)
6. Bonus: Find an error that could have real consequences
7. Bonus: Document system prompt failures or instruction-following problems

### Resources:
- Fact-checking websites list
- Deepfake detection tools
- AI error examples database
- Academic integrity guidelines

---

## ARCHIVE

###### ARCHIVE

**UPDATED 2025-06-02:** Enhanced with model naming confusion and system prompt failures

**Rationale:** Added critical new error types emerging in 2025: model naming confusion (Ollama mislabeling models) and system prompt failures (DeepSeek R1 ignoring instructions). Also included multilingual reasoning bias where AI performs worse in non-English languages. These represent current, real-world errors students encounter.

**Updated Content:**
- Enhanced section [seq:020] with Ollama model naming issues
- Updated section [seq:060] with DeepSeek R1 system prompt failures
- Enhanced section [seq:070] with multilingual reasoning bias
- Added instruction-following testing to homework
- Updated error categories to include modern failure modes

**New Error Types Added:**
- Model naming confusion: Tools calling different models than claimed
- System prompt failures: AI ignoring behind-the-scenes instructions
- Multilingual bias: Worse performance in non-English languages
- Instruction-following inconsistencies across models

**Educational Value:**
- Teaches students to verify what AI they're actually using
- Highlights importance of clear instruction-giving
- Raises awareness of language bias in AI systems
- Connects to real 2025 community discussions about model transparency

---

*End of Lecture 4*