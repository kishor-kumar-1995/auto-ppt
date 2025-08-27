# Your Text, Your Style – Auto-Generate a Presentation

Turn bulk text/markdown into a PowerPoint (.pptx) that matches a user-uploaded template’s style (colors, fonts, layouts, and images).  
**No AI image generation**; only reuse images from the template.

## Features (MVP)
- Paste long text or markdown
- Optional one-line guidance (e.g., “investor pitch deck”)
- User supplies their own LLM API key (OpenAI / Anthropic / Gemini) — never stored
- Upload a .pptx/.potx as style template
- Generate and download a new .pptx

## Tech Stack (planned)
- Backend: FastAPI (Python)
- Frontend: simple HTML (Jinja2) or minimal JS
- PPT handling: `python-pptx`
- LLM calls: `httpx` (provider-agnostic adapter)

## Security
- API keys are sent in the request and **not stored or logged**.

## Roadmap
- Speaker notes (via LLM)
- Previews before download
- Error handling & limits
