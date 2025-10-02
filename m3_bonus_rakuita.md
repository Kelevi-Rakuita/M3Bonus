# m3_bonus_rakuita.md — Prompts & Reflection

## Prompts / Conversation Highlights
- Starter prompt asking for step-by-step, minimal version first, and explanations.
- Clarifying Qs: why fixed number first; what `%` does; why pass-by-reference for attempts/score.
- Modifications: avoid `<random>`/`mt19937` and vectors; stick to `srand/rand` and cumulative totals.
- Correction: added robust input validation to prevent crashes on letters.

### Example Prompts You Can Reuse
- “Explain why you chose this approach before giving code.”
- “We haven’t learned arrays/classes yet—keep it to functions + if/switch.”
- “Can we add difficulty with a `switch` and a replay loop?”
- “Help me validate input so letters don’t crash the program.”

## Reflection (≈200 words)
I was surprised how helpful AI was at breaking the project into safe, testable steps. Starting with a fixed secret number seemed too simple at first, but it avoided confusion and made debugging easier once randomness was added. The hardest part was being precise about constraints—AI can’t guess what we’ve covered, so I had to say “no vectors or `<random>` yet” and ask for simpler alternatives. Once I asked the right questions, explanations about `rand()`, seeding, and input validation were clear, and the code felt approachable.

The easiest part was iterating: compile, test one small feature, then add the next. If I did this again, I would always ask AI to explain its design choices first and request a minimal version that fits the current module’s topics. Concepts that clicked were designing functions with clear inputs/outputs, pass-by-reference to return multiple results, using a `switch` for menus, and writing a `getValidatedInt` to keep input in range and protect against bad entries. AI acted like a helpful coach, but I still owned the debugging and decisions.

## Build & Run
```bash
g++ -std=c++11 m3bonus_rakuita.cpp -o m3bonus
./m3bonus
```

Include a terminal screenshot (after a round) as `screenshot.png` for Canvas.
