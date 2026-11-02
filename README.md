<img src="./assets/header-light.svg#gh-light-mode-only" alt="Samir Lorenzo, Junior Developer" width="100%" />
<img src="./assets/header-dark.svg#gh-dark-mode-only" alt="Samir Lorenzo, Junior Developer" width="100%" />

Full-stack developer based in Panama, open to on-site and remote roles.

[Email](mailto:samirherrera15@gmail.com) · [LinkedIn](https://www.linkedin.com/in/samirlorenzo)

## Selected work

<table>
<tr>
<td width="50%" valign="middle">
<a href="https://github.com/zSamir015/panama-canal-tracker"><img src="./assets/panama-canal-tracker.svg" alt="Panama Canal Tracker" width="100%" /></a>
</td>
<td width="50%" valign="middle">
<h3>Panama Canal Tracker</h3>
<p><em>In development</em></p>
<p>Tracks vessels around the Panama Canal from live AIS data.</p>
<ul>
<li>Worker ingests AIS messages and writes them in batches to TimescaleDB</li>
<li>Redis and WebSocket push updates to a MapLibre map</li>
<li>Argon2id, JWT and rate limiting protect the API</li>
<li>Python typed with mypy; design decisions recorded as ADRs</li>
</ul>
<p><a href="https://github.com/zSamir015/panama-canal-tracker/actions/workflows/ci.yml"><img src="https://github.com/zSamir015/panama-canal-tracker/actions/workflows/ci.yml/badge.svg" alt="Build status" /></a></p>
<p><a href="https://github.com/zSamir015/panama-canal-tracker">Code</a> · <a href="https://github.com/zSamir015/panama-canal-tracker/blob/main/docs/ARCHITECTURE.md">Architecture</a> · <a href="https://github.com/zSamir015/panama-canal-tracker/blob/main/docs/API_DESIGN.md">API</a> · <a href="https://github.com/zSamir015/panama-canal-tracker/tree/main/docs/adr">Decisions</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="middle">
<a href="https://zsamir015.github.io/obsidian-bank/"><img src="./assets/obsidian-bank.svg" alt="Obsidian Bank" width="100%" /></a>
</td>
<td width="50%" valign="middle">
<h3>Obsidian Bank</h3>
<p><em>Live</em></p>
<p>Online banking demo anyone can try without signing up.</p>
<ul>
<li>Balances change only after server-side validation</li>
<li>Row Level Security limits each user to their own data</li>
<li>Transfers, budgets, card freezing and web push alerts</li>
<li>English and Spanish, installable as a PWA, tested with Playwright</li>
</ul>
<p><a href="https://github.com/zSamir015/obsidian-bank/actions/workflows/ci.yml"><img src="https://github.com/zSamir015/obsidian-bank/actions/workflows/ci.yml/badge.svg" alt="Build status" /></a></p>
<p><a href="https://zsamir015.github.io/obsidian-bank/">Live demo</a> · <a href="https://github.com/zSamir015/obsidian-bank">Code</a> · <a href="https://github.com/zSamir015/obsidian-bank/blob/main/docs/USER_GUIDE.md">User guide</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="middle">
<a href="https://zsamir015.github.io/drafty/"><img src="./assets/drafty.svg" alt="Drafty" width="100%" /></a>
</td>
<td width="50%" valign="middle">
<h3>Drafty</h3>
<p><em>Live</em></p>
<p>Kanban board styled like a technical drawing, with no framework or build step.</p>
<ul>
<li>Drag and drop built on pointer events, not the HTML5 drag API</li>
<li>Board re-renders by reconciling keyed nodes</li>
<li>One state function handles history, saving and redraws</li>
<li>Works offline and with the keyboard</li>
</ul>
<p><a href="https://github.com/zSamir015/drafty/actions/workflows/test.yml"><img src="https://github.com/zSamir015/drafty/actions/workflows/test.yml/badge.svg" alt="Build status" /></a></p>
<p><a href="https://zsamir015.github.io/drafty/">Live demo</a> · <a href="https://github.com/zSamir015/drafty">Code</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="middle">
<a href="https://zsamir015.github.io/brutus/"><img src="./assets/brutus.svg" alt="Brutus" width="100%" /></a>
</td>
<td width="50%" valign="middle">
<h3>Brutus</h3>
<p><em>Live</em></p>
<p>Landing page for a fictional burger joint in Costa del Este.</p>
<ul>
<li>Plain HTML, CSS and JavaScript modules</li>
<li>Supabase Edge Function validates and rate-limits signups</li>
<li>Filterable menu and live opening hours</li>
<li>Tests and Lighthouse checks run in CI</li>
</ul>
<p><a href="https://github.com/zSamir015/brutus/actions/workflows/test.yml"><img src="https://github.com/zSamir015/brutus/actions/workflows/test.yml/badge.svg" alt="Build status" /></a></p>
<p><a href="https://zsamir015.github.io/brutus/">Live demo</a> · <a href="https://github.com/zSamir015/brutus">Code</a></p>
</td>
</tr>
</table>

<details>
<summary>Panama Canal Tracker architecture</summary>

```mermaid
flowchart LR
    A[AIS feed or simulator] --> B[Ingestion worker]
    B --> C[(TimescaleDB)]
    B --> D[(Redis)]
    C --> E[FastAPI]
    D --> E
    E -->|WebSocket| F[React and MapLibre map]
```

</details>

## Stack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=ts%2Cjs%2Cpython%2Cswift%2Cjava%2Ccs%2Ccpp%2Creact%2Cfastapi%2Csupabase%2Cpostgres%2Credis%2Cdocker%2Cgithubactions&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://skillicons.dev/icons?i=ts%2Cjs%2Cpython%2Cswift%2Cjava%2Ccs%2Ccpp%2Creact%2Cfastapi%2Csupabase%2Cpostgres%2Credis%2Cdocker%2Cgithubactions&theme=light">
  <img alt="Stack" src="https://skillicons.dev/icons?i=ts,js,python,swift,java,cs,cpp,react,fastapi,supabase,postgres,redis,docker,githubactions&theme=light">
</picture>
