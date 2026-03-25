# Sales Consultant Chatbot — Project Context

## Project Overview

This is a **single-page portfolio project** showcasing an AI-powered Sales Assistant Chatbot. The project is a static HTML page that serves as both a presentation of the product concept and a functional demo of the chatbot interface.

**Purpose:** Demonstrate an AI sales enablement tool that helps Sales Consultants get instant, intelligent responses during customer interactions.

**Type:** Static web page (HTML/CSS/JavaScript) — no build process or dependencies required.

## Tech Stack

- **HTML5** — Semantic structure
- **CSS3** — Custom styling with CSS variables, animations, and responsive design
- **Vanilla JavaScript** — Interactive chatbot demo (no frameworks)
- **Google Fonts** — DM Serif Display and DM Sans

## File Structure

```
sales_consultant_chatbot/
└── index.html    # Single-file application (HTML + CSS + JS)
```

## Key Features

### Presentation Layer
- Hero section with project overview
- Stakeholder identification (Sales Consultants, Sales Managers, Customers)
- Problem statement and opportunity
- Solution proposal (AI Sales Assistant)
- Benefits breakdown (for consultants and businesses)
- How-it-works section with 4-step process flow
- Optional advanced features (Voice-to-Text, CRM Integration, Performance Feedback)

### Interactive Chatbot Demo
- Floating action button (FAB) to open/close the chat
- Three pre-configured sales scenarios:
  1. **Price objection** — Handling "too expensive" concerns
  2. **Stalling customer** — Moving hesitant buyers forward
  3. **Upsell opportunity** — Cross-selling after a sale
- Simulated AI response with typing indicator
- Status indicator (active/loading states)

## Running the Project

**No build required.** Simply open `index.html` in a web browser:

```bash
# Option 1: Direct file open
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows

# Option 2: Local server (recommended for full functionality)
python -m http.server 8000
# Then visit: http://localhost:8000
```

## Design System

### CSS Variables
| Variable | Value | Usage |
|----------|-------|-------|
| `--bg` | `#F7F6F3` | Page background |
| `--surface` | `#FFFFFF` | Card/surface backgrounds |
| `--border` | `#E2E0DA` | Borders and dividers |
| `--text` | `#1A1916` | Primary text |
| `--muted` | `#6B6860` | Secondary/muted text |
| `--subtle` | `#EDECE8` | Subtle backgrounds |
| `--ink` | `#2C2A27` | Dark accents, buttons |
| `--rule` | `#D4D2CC` | Rules and decorative elements |

### Typography
- **Serif:** DM Serif Display — Headlines, hero titles
- **Sans-serif:** DM Sans — Body text, UI elements

## JavaScript Architecture

### Key Functions
| Function | Purpose |
|----------|---------|
| `toggleChat()` | Opens/closes the chat popup |
| `cpAsk()` | Handles chat submission with simulated AI delay |
| `cpAppend(role, text)` | Adds a message bubble to the chat |
| `cpShowTyping()` / `cpRemoveTyping()` | Shows/hides typing indicator |
| `cpSetStatus(text, mode)` | Updates status text and indicator dot |

### Chat Flow
1. User selects a scenario pill
2. Clicks "Ask" button
3. User message is appended to chat
4. Typing indicator appears (1-second delay)
5. Pre-configured response is displayed
6. Status returns to "Ready"

## Responsive Behavior

- **Desktop (>860px):** Two-column hero layout, full navigation
- **Mobile (≤860px):** Single-column layout, hidden nav links, adjusted chat positioning

## Future Enhancement Opportunities

If extending this project, consider:
- Connecting to a real AI API (e.g., OpenAI, Anthropic)
- Adding more sales scenarios dynamically
- Implementing conversation history
- Adding CRM integration mockups
- Including analytics/tracking for demo engagement

## Notes for Development

- All code is in a single file — edits should maintain the inline structure
- CSS is organized by section comments (e.g., `/* ── NAV ───────────────────── */`)
- JavaScript uses vanilla ES5+ syntax with no transpilation needed
- The chatbot responses are hardcoded in the `responses` object — replace with API calls for production use
