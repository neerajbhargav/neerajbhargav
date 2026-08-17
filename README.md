## Neeraj Bhargav Rondla

**Applied AI Engineer** · Jersey City, NJ · [neerajbhargav.com](https://neerajbhargav.com)

I take ambiguous problems from zero to production AI systems and own them end to end: retrieval, agents, evaluation, the interface, and the infrastructure underneath. No handoffs.

Currently the sole AI engineer at **Landair Advisors** (NYC commercial real estate), where I own five production AI systems. Targeting **Forward Deployed Engineer** roles.

### The part I actually care about: evaluation

I have twice killed my own improvements because the measurement said no.

After single-run variance produced two false wins, I instituted a 3-run protocol. The first thing it did was reject a larger-model upgrade I had personally championed, because it measured 14 points worse. The same protocol later surfaced a name-parser inversion silently corrupting 69% of records; the fix tripled exact-match accuracy from 16% to 48%.

The pipeline it guards went from a ~50% manual baseline to **93.3% accuracy** over a 1,121-record run, at roughly $8-15 per 2,000 records. Confidently-wrong output sits at zero in production, because low-confidence results get flagged for human review instead of returned silently.

Anyone can ship a pipeline that looks good on one run. Building the harness that tells you the truth, and then obeying it when it says no, is the part most people skip.

### Open source: MCP and agent tooling

**[vibetter](https://github.com/neerajbhargav/vibetter)** · Python, FastMCP 3.0
MCP server for Claude Code, Cursor, Windsurf and Claude Desktop. Git-diff explanation with contextual reasoning, source-grounded Q&A with `file:line` citations, codebase-aware debugging, and an interactive dependency graph. Multi-provider: Anthropic, OpenAI, Gemini, or local Ollama.

**[omni-context](https://github.com/neerajbhargav/omni-context)** · TypeScript, MCP SDK
MCP bridge and session handoff for AI coding assistants. A local daemon compresses git state and active tasks into a portable handoff prompt, and a native MCP server exposes a `context://current` resource so Cursor and Claude Code can read project state directly.

**[context-refinery](https://github.com/neerajbhargav/context-refinery)** · Python, LangGraph
Multi-agent context engine: intent analysis, hybrid retrieval (dense + BM25 + RRF), cross-encoder reranking, and eval-gated self-refinement scored by custom local metrics (n-gram grounding, information density, budget utilization), with optional DeepEval / RAGAS when a cloud API key is set. Runs fully offline via Ollama.

### Stack

**LLMs, agents, MCP** Claude API (Sonnet, Opus, Haiku, Vision) · GPT-4/4o · Gemini · Llama · Model Context Protocol · FastMCP · MCP SDK · LangGraph · LangChain · DSPy · ReAct · multi-agent orchestration · human-in-the-loop

**Retrieval and evaluation** RAG · agentic RAG · hybrid retrieval (BM25 + dense + RRF) · cross-encoder reranking · pgvector · ChromaDB · Pinecone · FAISS · RAGAS · DeepEval · LangSmith · LLM-as-judge · faithfulness and hallucination scoring · drift monitoring · guardrails · prompt-injection defense

**Engineering** Python · TypeScript · SQL · FastAPI · Pydantic · Node.js · PostgreSQL · Redis · asyncio · Docker · AWS · GitHub Actions · React · Next.js

### Writing

- [Forward-Deployed: Shipping Five AI Systems Zero-to-One](https://neerajbhargav.com/writing/forward-deployed-five-systems)
- [An Agent You Can't Measure Is One You Can't Trust](https://neerajbhargav.com/writing/eval-harness-trust)
- [When Verification Is the Product](https://neerajbhargav.com/writing/cross-verification-product)

---

M.S. Computer Science, NJIT · B.Tech CSE, JNTUH · OPT / STEM extension eligible

[Portfolio](https://neerajbhargav.com) · [LinkedIn](https://www.linkedin.com/in/neerajbhargav) · [X](https://x.com/neerajbhargav_r) · rondlanbr@gmail.com
