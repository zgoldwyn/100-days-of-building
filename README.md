# 100 Days of Building

A daily experiment in building small, self-contained browser projects.

Each day, a GitHub Actions workflow uses an LLM API to generate one new project using plain HTML, CSS, and JavaScript. Projects may include mini-games, puzzles, simulations, creative tools, visualizations, productivity tools, and other interactive ideas.

## Goals

- Build and explore a wide variety of small project ideas
- Practice reading, testing, modifying, and improving generated code
- Maintain a consistent daily building habit
- Create a growing archive of interactive experiments

## Project Structure

Each generated project is stored in its own dated folder:

```text
projects/
├── 2026-07-30-example-project/
│   ├── index.html
│   └── README.md
└── README.md
```

Open a project's `index.html` file in a browser to run it.

## Automation

The workflow in `.github/workflows/daily-project.yml`:

1. Reviews recent project README files to avoid duplicates
2. Generates a new project idea and implementation
3. Creates a dated project folder
4. Updates the project index
5. Commits the new project to the repository

It expects these workflow settings:
- Repository secret: `OPENAI_API_KEY`
- Model env var in workflow: `LLM_MODEL` (default `gpt-4.1-mini`)

## AI Disclosure

The initial versions of these projects are generated automatically using a configured LLM model. I review, test, modify, and improve projects when possible.

## Project Index

See [`projects/README.md`](./projects/README.md) for the complete list of generated projects.
