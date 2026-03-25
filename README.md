# Sales Consultant Chatbot

An AI-powered Sales Assistant Chatbot portfolio project that demonstrates a real-time sales enablement tool. This static web application showcases how AI can help Sales Consultants get instant, intelligent responses during customer interactions.

## 🎯 Purpose

This project demonstrates an AI sales enablement tool designed to help Sales Consultants:
- Get instant answers to customer questions
- Handle objections confidently
- Discover upsell and cross-sell opportunities
- Deliver consistent messaging across all customer interactions

## ✨ Features

### Presentation Layer
- **Hero Section** — Interactive 3D scene with orbiting elements (Three.js)
- **Stakeholder Identification** — Sales Consultants, Sales Managers, Customers
- **Problem & Opportunity** — Clear articulation of sales challenges
- **Solution Proposal** — AI Sales Assistant breakdown
- **Benefits** — For both consultants and businesses
- **How It Works** — 4-step process flow with optional advanced features

### Interactive Chatbot Demo
- **Floating Action Button (FAB)** — Opens/closes the chat interface
- **3 Pre-configured Sales Scenarios:**
  1. Price objection handling
  2. Stalling customer management
  3. Upsell opportunity identification
- **Simulated AI Responses** — Typing indicator with realistic delay
- **Status Indicator** — Active/loading states with animated glow effect

### UI/UX Enhancements
- **3D Hero Animation** — Four images orbit around the central card in 3D space
- **Interactive Rotation** — Click and drag to rotate the 3D scene
- **Glowing Status Dot** — Pulsing indicator for chat state
- **Button Hover Effects** — Smooth transitions and shadows
- **Sound Effects** — Subtle chimes for send/receive actions
- **Responsive Design** — Works on desktop and mobile devices

## 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML5 | Semantic structure |
| CSS3 | Custom styling with CSS variables, animations |
| Vanilla JavaScript | Interactive chatbot (no frameworks) |
| Three.js (r128) | 3D hero section animation |
| Google Fonts | DM Serif Display & DM Sans |
| Web Audio API | Sound effects (no external audio files) |

## 📁 File Structure

```
sales_consultant_chatbot/
├── index.html          # Single-file application (HTML + CSS + JS)
├── README.md           # Project documentation
└── QWEN.md             # Project context & design system
```

## 🚀 Getting Started

No build process or dependencies required. This is a static web application.

### Option 1: Direct File Open
```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

### Option 2: Local Server (Recommended)
```bash
# Using Python 3
python -m http.server 8000

# Then visit: http://localhost:8000
```

### Option 3: Using Node.js
```bash
npx serve .
```

## 🎨 Design System

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

## 🎮 Chatbot Interaction

### How to Use the Demo
1. Click the floating **"Chat"** button in the bottom-right corner
2. Select one of the three scenario pills
3. Click **"Ask"** to see the AI response
4. Listen for subtle sound effects on send/receive

### Sound Effects
- **Send chime** (D5→G5): Plays when you submit a question
- **Receive chime** (C5→E5): Plays when the assistant responds

> 💡 Note: Sounds require user interaction first due to browser autoplay policies.

### 3D Hero Scene
- **Auto-rotation:** Images orbit continuously in a diamond pattern
- **Drag to interact:** Click and drag to speed up or reverse rotation
- **Release:** Returns to smooth auto-rotation

## 📱 Responsive Behavior

| Breakpoint | Behavior |
|------------|----------|
| **Desktop (>860px)** | Two-column hero layout, full navigation |
| **Mobile (≤860px)** | Single-column layout, hidden nav links, adjusted chat positioning |

## 🔮 Future Enhancements

Potential improvements for this project:

- [ ] Connect to a real AI API (OpenAI, Anthropic, etc.)
- [ ] Add more sales scenarios dynamically
- [ ] Implement conversation history
- [ ] CRM integration mockups
- [ ] Voice-to-text input capability
- [ ] Analytics/tracking for demo engagement
- [ ] Dark mode toggle
- [ ] Export conversation functionality

## 📄 License

This is a portfolio project for demonstration purposes. Feel free to use as inspiration for your own projects.

## 🤝 Contact

For questions or feedback about this project, please open an issue on GitHub.

---

**Built with** ❤️ **using Three.js, Web Audio API, and Vanilla JavaScript**
