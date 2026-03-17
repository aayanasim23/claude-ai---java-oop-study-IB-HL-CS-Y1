# IB CS OOP // TERMINAL

> Java OOP exam prep for IB Computer Science HL — Option D

Live at → **[aayanasim23.github.io/claude-ai---java-oop-study-IB-HL-CS-Y1](https://aayanasim23.github.io/claude-ai---java-oop-study-IB-HL-CS-Y1/)**

---

## What it is

A focused study tool built specifically for **IB CS HL Option D (Object-Oriented Programming)**. No fluff, no ads, no account required to use.

The question bank is built directly from real IB past papers (2016, 2017) and covers every concept that consistently shows up in Paper 2 Option D:

- Inheritance, IS-A vs HAS-A relationships
- Method overriding vs overloading
- Encapsulation, private fields, accessor methods
- Static vs instance variables and methods
- Constructors, `super()`, constructor chaining
- UML class diagrams
- Array of objects — search, filter, max patterns
- Subclass construction with `super()`
- LinkedList vs array discussion
- Binary tree traversal (inorder, postorder)
- Output tracing across all of the above

---

## Features

| Feature | What it does |
|---|---|
| **5 study modes** | Output Tracing / Concepts / Write Code / Full Mix / IB Paper 2 Sim (20min timed) |
| **Wrong answer drill** | Automatically re-queues questions you get wrong |
| **Anti-repetition engine** | Prioritises questions you haven't seen recently |
| **AI grading** | Checks your written answers and code using your own API key |
| **AI Unlimited mode** | Generates infinite new questions on demand |
| **Progress sync** | Signs in with Google, syncs progress across devices via Supabase |
| **Works offline** | Progress saved to localStorage, syncs when back online |

---

## AI grading setup

The AI grading feature uses your own API key — nothing is stored server-side. Supports:

| Provider | Free tier | Get key |
|---|---|---|
| **Groq** | 1000 req/day, no card | [console.groq.com](https://console.groq.com) |
| **Gemini** | Generous free tier | [aistudio.google.com](https://aistudio.google.com) |
| **OpenRouter** | 50 free req/day | [openrouter.ai](https://openrouter.ai) |
| OpenAI | Paid | [platform.openai.com](https://platform.openai.com) |
| Anthropic | Paid | [console.anthropic.com](https://console.anthropic.com) |

Groq or Gemini is the recommended starting point — both are free and require no credit card.

---

## How it works

The entire app is a single `index.html` file:

- **Frontend** — hosted on GitHub Pages (free, no server needed)
- **Backend/Database** — [Supabase](https://supabase.com) handles auth (Google OAuth) and progress storage with Row Level Security (each user only accesses their own data)
- **AI calls** — made directly from your browser to whichever provider key you configure. Keys never leave your device and are never stored in the database.

---

## Tech stack

```
HTML / CSS / Vanilla JS    — no frameworks, no build step
Supabase                   — auth + Postgres DB
Google OAuth               — sign in
GitHub Pages               — hosting
Groq / Gemini / OpenRouter — AI grading (user's own key)
```

---

## Question bank

60+ questions covering the full IB Option D syllabus, including:

- 12 output tracing questions
- 12 concept MC questions  
- 4 written definition questions
- 10 code-writing questions
- 22 questions built directly from 2016 and 2017 IB past papers

---

## Contributing

If you're an IB CS student and want to add questions, open a PR. Question format is a JS object in `BANK` array — see existing questions for the pattern. All questions should be based on real IB past paper patterns or the official syllabus.

---

## About

Built by an IB CS HL student, for IB CS HL students. Made because the existing study tools either don't cover Java OOP specifically or make you pay for flashcard apps.

If this helped you pass, feel free to star the repo.

---

*Not affiliated with the IBO. All past paper content referenced for educational purposes.*
