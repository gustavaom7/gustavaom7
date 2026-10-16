# Portfolio backlog

Open work from the portfolio audit of October 2026. Target: Senior QA Automation Engineer (AI-focused), international remote. Budget: about 10 h/week.

Already done (Oct 2026): XCUITest CI fixed (19/19 green), Maestro CI green with honest docs, RestAssured "security" tests renamed to input handling, Cypress and profile links fixed, RestAssured Allure report published on Pages.

## LinkedIn and GitHub profile

- [x] LinkedIn headline, Top Skills (Playwright, Test Automation, TypeScript) and About line breaks.
- [ ] Pinned repos: Playwright, Appium, Cypress, RestAssured, Maestro, portfolio site.

## CVs

The four CV PDFs (Automation, QA Engineer, Mobile, Manual) are edited outside this repo.

- [ ] Add **Java** (RestAssured, JUnit 5) and **Python** (pytest, LLM tooling) to the skills line. Both have public proof: `api-testing-restassured`, `maestro-mobile-ai-qa`.
- [ ] Add **WebdriverIO** next to Appium (ATS keyword, proven in `appium-mobile-e2e-framework`).
- [ ] Add the portfolio URL `gustavaom7.github.io` to the header of all four CVs.
- [ ] **Selenium:** drop it, or prove it (Selenium 4 + JUnit in the Java repo, about 4 h).
- [ ] **Docker:** drop it, or prove it (run one suite in a container in CI).
- [ ] **GitLab CI:** keep only if used at work; never lead with it.
- [ ] Replace the CV hosted on the site (`GustavoMesquita-QAEngineer-CV.pdf`) with the updated version.

## Roadmap (12 weeks)

### Weeks 3–4 · Python
- [ ] Maestro flow generator: pytest tests, typed config, retries, cost logging.
- [ ] Measure the generator: 10 generated flows, lines edited before each passes; publish the number in the README.

### Weeks 5–8 · New flagship repo: `llm-eval-qa`
- [ ] Small RAG chatbot over public docs as the system under test.
- [ ] promptfoo regression suite: golden questions, factuality/faithfulness, refusals, output format.
- [ ] DeepEval or Ragas metrics in pytest; red-team pass (prompt injection, data leakage).
- [ ] Cost and latency budgets as CI gates; Langfuse traces for failures.
- [ ] README: risk-based test strategy for LLM features, written for a product manager.

### Weeks 9–10 · API and data
- [ ] RestAssured: Testcontainers (Postgres + WireMock), SQL assertions, attack payloads against the local target only.
- [ ] Pact consumer/provider pair, or Schemathesis against an OpenAPI spec.
- [ ] Run one suite inside a Docker image in CI.

### Week 11 · Device cloud
- [ ] Appium iOS smoke on BrowserStack (open-source plan) or a `macos-15` simulator job.

### Week 12 · Visibility
- [ ] Two articles: "Deterministic triage before LLM triage" and "Regression-testing an LLM feature like a k6 budget".
- [ ] Update the site case study, this README and the CVs with the new repo and numbers.
- [ ] Optional: ISTQB CT-GenAI.

## Smaller follow-ups

- [ ] Maestro: its workflow runs only on PRs and on demand, so its badge has no `main` status. Run it once on `main`, then add its CI badge to the profile table.
- [ ] Maestro: `09_change_text_size` taps through 50% → 100% on every run although `clearState` already resets the size; asserting `100% (Default)` directly would save up to 10 minutes of CI.
- [ ] Playwright: review and commit the visual-regression baselines so `@visual` can gate CI.
- [ ] Add one business number to each flagship README (run time, cost, failures triaged).
- [ ] Add a short "How I work with AI" note to this profile README (what the agent drafts, what I review).
