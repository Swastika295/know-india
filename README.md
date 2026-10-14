# Know India

A royal-themed civics almanac of India. Browse the Constitution, explore the states, take an endless governance quiz, and ask AI about world affairs. The whole site is a single HTML file with no build step.

## Features

| Section | What it does |
|---|---|
| **Constitution** | Searchable list of 27 key articles and 16 amendments. Tap any item to read more, open its Wikipedia page, or ask AI for a deeper explanation. |
| **States** | All 28 states with capital, area, languages and culture. Pick a state and ask a question about it. |
| **Governance** | Quiz on Parliament, the executive, the judiciary and elections. It has no fixed length, shows the correct answer and an explanation after every question, and keeps going until you stop clicking Next. |
| **World Affairs** | Chat about international relations and policy, answered in a neutral, encyclopedic style. |

## Run locally

Open `index.html` in any web browser. There is nothing to install.

## Deploy

This site is deployed on [Vercel](https://vercel.com). To deploy your own copy:

1. Rename `know-india.html` to `index.html` and put it in a GitHub repository.
2. In Vercel, choose **Add New**, then **Project**, and import the repository.
3. Leave the framework preset as **Other**, with no build command, then click **Deploy**.

Every commit you push to the repository redeploys the site automatically.

## About the AI features

The AI features were built for the page published on Claude, which provides the AI connection. They are:

- state questions
- "Explain in depth" in the Constitution section
- the World Affairs chat
- AI-generated quiz questions

When the file is hosted elsewhere, these features are unavailable. The state box falls back to a built-in summary, and the quiz repeats its built-in questions.

To enable them on your own host, add a small server-side function (for example a Netlify Function or Cloudflare Worker) that calls an AI API, and change the page to call that function. Keep your API key on the server and never put it in the HTML file.

## About the data

Reference content (articles, amendments, state facts, quiz questions) is a built-in snapshot written to follow Wikipedia. It is not fetched live and may contain mistakes or become outdated. Each section links to Wikipedia for the latest text. AI-generated answers can also be incomplete or wrong, so check important facts against reliable sources.

## Built with

Plain HTML, CSS and JavaScript. Fonts are Cinzel and EB Garamond from Google Fonts, with Georgia as a fallback.

## Author

Created by Swastika Singh
