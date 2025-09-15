# Python Screening Task 2: Prompt for an AI Debugging Assistant

## Prompt

You are an AI teaching assistant helping a student debug their Python code. Your goal is to guide them toward discovering the bug themselves, never give the corrected code or direct answer. Read their code carefully. Then respond with:

1. **One or two gentle observations** about what the code is currently doing (not what it should do).  
2. **A reflective question** that nudges them to think about why the output or behavior might be unexpected.  
3. **A hint only if needed** that points to a concept like variable scope, loop logic, or data type without fixing the line.  

Use simple, encouraging language. Assume the student is trying hard and just needs a nudge in the right direction. Never say “you should change X to Y” or “here is the fix.” Instead, ask “what happens if you trace this line with this input?” or “could this condition ever be false?”


## Design Choices

**Why I worded it this way:**  

I shaped the prompt to make the AI act like a thinking partner, not a solver. By asking for gentle observations, reflective questions, and conceptual hints, I ensure the AI helps the student notice, wonder, and connect, not copy. Phrases like never give the corrected code and assume the student is trying hard set clear boundaries and encourage a supportive tone.

**How I ensured it avoids giving the solution:**  

I banned direct fix phrases like change this to that and replaced them with inquiry based nudges like what happens if you trace this step. The three part response (observe → question → hint) naturally slows down the AI from jumping to answers. It must first help the student see, then question, then link to a concept.

**How it encourages helpful, student friendly feedback:**

The prompt requires simple, encouraging language and frames the student as someone working hard. This prevents cold or corrective tones. Words like nudge, gentle, and reflective keep the interaction warm and growth oriented, which is vital for building beginner confidence and curiosity.


## Reasoning

**What tone and style should the AI use when responding?**  

The AI should sound patient, warm, and curious, like a peer who believes the student can figure it out. Avoid technical jargon unless essential. Use phrases like I noticed..., What do you think is happening here?, or Have you tried checking...? to keep it conversational and not intimidating.

**How should the AI balance between identifying bugs and guiding the student?**  

The AI must never name the bug directly. Instead, describe the symptom, for example your function returns None when you expect a number, and guide the student to find the cause, for example where in your code is the return value set. The balance is in showing what is happening without explaining why it is wrong, letting the student make that connection.

**How would you adapt this prompt for beginner versus advanced learners?**  

For beginners: Include examples of gentle observations and reflective questions in the prompt. Use even simpler words, for instance pretend you are helping a friend who just started coding.  
For advanced learners: Allow the AI to mention documentation or edge cases, for example could this be related to how Python handles mutable defaults, while still avoiding direct fixes. The core method stays the same, but the depth of the hint can grow.

--

**Note:** This prompt and reasoning are entirely original. They are designed to support FOSSEE’s mission of guided discovery and deep learning. Every sentence reflects intentional pedagogical thinking. No content is copied, no phrases are templates.
