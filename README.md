## Neeraj Bhargav Rondla

Applied AI Engineer in New York. I make AI systems provably accurate in production.

I'm the sole AI engineer at Landair Advisors, a NYC commercial real estate brokerage. I run five production AI services there. The headline one is an agentic Claude pipeline that finds the person behind LLC-owned buildings. It is 97.1% accurate on 1,088 of 1,120 labeled properties, up from a ~50% manual baseline. I've merged 834 PRs across 4 repos since June 2026.

The habit I care about most is an eval that can say no. A 3-run test on a 15-row labeled set rejected my own model upgrade (53% vs 67%), and it showed that two earlier "wins" were single-run noise.

**Start here**

- [vibetter](https://github.com/neerajbhargav/vibetter): an MCP server for Claude Code and Cursor that machine-checks every file:line citation it gives. On 66 questions over three pinned open-source repos, its retrieval puts the answer's code in front of the model 83% of the time, where the first version managed 0%.
- [sidegig](https://github.com/neerajbhargav/sidegig): a free, open-source browser sidebar and new tab with your signed-in apps and an AI assistant. Its sign-in code detector went from 53.3% to 77.3% recall at 96.7% precision on a 330-email held-out set.
- [splitter](https://github.com/neerajbhargav/splitter): shared expenses and personal finance, exact to the cent. It enforces Postgres row-level security on every table and passes 341 offline tests. Live at [usesplitter.vercel.app](https://usesplitter.vercel.app).

**Writing:** [An Agent You Can't Measure Is One You Can't Trust](https://neerajbhargav.com/writing/eval-harness-trust) | [Forward-Deployed: Operating Five AI Systems End-to-End](https://neerajbhargav.com/writing/forward-deployed-five-systems)

[neerajbhargav.com](https://neerajbhargav.com) | [LinkedIn](https://www.linkedin.com/in/neerajbhargav) | [X](https://x.com/nebhron) | rondlanbr@gmail.com
