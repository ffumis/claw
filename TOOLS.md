# TOOLS.md - Local Notes

## API Keys

All keys stored in `.env` (gitignored). Load with `source .env` or `export $(cat .env | grep -v '^#' | xargs)`.

| # | Service | Env Var | Use Case |
|---|---------|---------|----------|
| 1 | **GitHub** | `GITHUB_PAT` | Push/pull to `ffumis/claw` repo, create repos, manage issues |
| 2 | **Anthropic** | `CLAUDE_OAUTH_KEY` | Claude API access (coding agents, Claude Code) |
| 3 | **OpenAI** | `OPENAI_OATH_TOKEN` | GPT models, DALL-E, Whisper API |
| 4 | **xAI** | `XAI_API_KEY` | Grok models |
| 5 | **Google** | `GOOGLE_API_KEY` | Gemini, Google AI services |
| 6 | **Mem0** | `MEM0_API_KEY` | Long-term memory storage/retrieval |
| 7 | **Pinecone** | `PINECONE_API_KEY` | Vector database for embeddings/RAG |
| 8 | **Hyperbrowser** | `HYPERBROWSER_API_KEY` | Browser automation, web scraping |
| 9 | **Tavily** | `TAVILY_API_KEY` | AI-powered web search |
| 10 | **Firecrawl** | `FIRECRAWL_API_KEY` | Web crawling & scraping |
| 11 | **Financial Modelling Prep** | `FMP_API_KEY` | Stock data, financial statements, market info |
| 12 | **Modal** | `MODAL_API_KEY` | Serverless compute (run GPU jobs, deploy functions) |
| 13 | **Telegram** | `TELEGRAM_BOT_TOKEN` | Bot messaging (already connected via OpenClaw) |

## GitHub

- **Repo:** https://github.com/ffumis/claw (public)
- **User:** ffumis (Ricky Chan)
- **PAT embedded in git remote** — remote URL includes token for auth

## Notes

- `.env` is gitignored — never commit it
- Keys were set up 2026-03-22
- Rotate keys periodically, especially GitHub PAT
