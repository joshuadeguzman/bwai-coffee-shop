# bwai-coffee-shop

Sample Firebase Genkit flows for an AI-powered coffee shop, used at Build with AI. It shows how to write prompts and flows in Genkit with Gemini.

## Flows

| Flow | What it does |
|---|---|
| `simpleGreeting` | Greets a customer by name and recommends a drink. |
| `greetingWithHistory` | Greets a returning customer using the time of day and their previous order, with a multi-message prompt. |
| `testAllCoffeeFlows` | Runs both flows with sample input. |

All flows are in `src/index.ts`. Sample input is in `src/input.json`.

## Running it

```bash
export GOOGLE_GENAI_API_KEY=<your key>
npm install
npm run genkit:dev
```

This opens the Genkit developer UI, where you can run each flow and inspect its traces. Get an API key from [Google AI Studio](https://aistudio.google.com/apikey).

## Stack

TypeScript, [Firebase Genkit](https://firebase.google.com/docs/genkit) and Gemini through the Google AI plugin.
