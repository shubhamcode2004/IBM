# 💡 Smart Business Idea Generator Agent

> An IBM Hackathon-grade AI-powered platform that transforms simple prompts into structured, market-ready business opportunities using **Agentic AI** and **Generative AI**.

---

## 🚀 Overview

The **Smart Business Idea Generator Agent** is a single-page web application that intelligently combines knowledge from research papers, articles, industry reports, market trends, and social media insights to generate high-quality, relevant, and actionable business ideas.

Rather than producing random suggestions, the platform analyzes user intent, current market demand, emerging technologies, and future trends — then delivers structured business concepts with full supporting analysis.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🎙️ **Multimodal Input** | Accept text, voice notes, images, product sketches, and documents |
| 🧠 **IBM Granite Intelligence** | Enterprise-grade reasoning via IBM Granite foundation models |
| 📈 **Real-time Market Trends** | Monitors research papers, industry reports, social media, and news |
| 🗺️ **Implementation Roadmaps** | Auto-generated go-to-market plans with timelines and KPIs |
| 🔀 **Agentic AI Orchestration** | IBM Orchestrate agents autonomously research, validate, and score ideas |
| 📊 **SWOT + Business Canvas** | Full SWOT analysis and Business Model Canvas for every idea |
| 🔮 **Innovation Scoring** | Proprietary engine scoring innovation, feasibility, and market impact |
| 🌐 **Langflow Pipelines** | Visual AI workflow automation for multi-step reasoning chains |
| 🎨 **Interactive Dashboard** | Mind maps, impact matrices, feasibility charts, and business canvases |
| 🌙 **Light / Dark Mode** | Smooth theme toggle with preference saved to localStorage |
| 📱 **Fully Responsive** | Mobile-first layout — works on all screen sizes |

---

## 🏗️ Technology Stack

### IBM Core Technologies (Mandatory)
| Technology | Role |
|---|---|
| **IBM watsonx.ai** | Core AI runtime and model hosting |
| **IBM Granite Models** | Language understanding and business idea generation |
| **IBM Langflow** | Visual AI workflow orchestration (multi-step pipelines) |
| **IBM Orchestrate** | Multi-agent automation — research, scoring, synthesis agents |

### Frontend
| Technology | Role |
|---|---|
| **React** | Component-based UI framework |
| **Next.js** | Server-side rendering and routing |
| **Tailwind CSS** | Utility-first responsive styling |
| **Framer Motion** | Smooth animations and transitions |
| **Lucide Icons** | Clean, modern icon set |
| **Chart.js** | Innovation score charts and analytics visuals |

### Backend & Data
| Technology | Role |
|---|---|
| **Node.js** | Server runtime |
| **Express.js** | REST API layer |
| **MongoDB** | Idea storage and user workspace data |
| **Firebase Authentication** | Secure user login and session management |

---

## 📁 Project Structure

```
smart-business-idea-generator/
├── index.html              # Main landing page (self-contained)
├── README.md               # Project documentation
├── assets/
│   ├── css/                # Additional stylesheets (if extracted)
│   └── js/                 # Additional scripts (if extracted)
├── src/
│   ├── components/         # React components (for full build)
│   │   ├── Hero.jsx
│   │   ├── Features.jsx
│   │   ├── Dashboard.jsx
│   │   ├── AICapabilities.jsx
│   │   ├── HowItWorks.jsx
│   │   └── ...
│   ├── pages/              # Next.js pages
│   │   └── index.js
│   └── lib/
│       ├── watsonx.js      # IBM watsonx.ai API integration
│       ├── langflow.js     # IBM Langflow pipeline calls
│       └── orchestrate.js  # IBM Orchestrate agent triggers
├── api/
│   ├── generate.js         # Idea generation endpoint
│   ├── analyze.js          # Market analysis endpoint
│   └── score.js            # Innovation scoring endpoint
└── .env.example            # Environment variable template
```

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js v18+
- npm or yarn
- IBM Cloud account with watsonx.ai access
- MongoDB instance (local or Atlas)
- Firebase project

### 1. Clone the Repository
```bash
git clone https://github.com/your-org/smart-business-idea-generator.git
cd smart-business-idea-generator
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment Variables
```bash
cp .env.example .env
```

Edit `.env` with your credentials:
```env
# IBM watsonx.ai
WATSONX_API_KEY=your_watsonx_api_key
WATSONX_PROJECT_ID=your_project_id
WATSONX_URL=https://au-syd.ml.cloud.ibm.com

# IBM Orchestrate
ORCHESTRATE_ORCHESTRATION_ID=a17f3124901d4027a3b9bf411860fdc3_83b4226c-ef1b-47ca-8096-af2e048a0f5b
ORCHESTRATE_HOST_URL=https://au-syd.watson-orchestrate.cloud.ibm.com
ORCHESTRATE_AGENT_ID=9410d9da-685f-421f-ab6c-4ad3863df6cd
ORCHESTRATE_AGENT_ENV_ID=225d8b3a-8599-4b3d-b249-0034b6f8de3c

# IBM Langflow
LANGFLOW_API_URL=your_langflow_api_url
LANGFLOW_API_KEY=your_langflow_api_key

# MongoDB
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/ideagenai

# Firebase
FIREBASE_API_KEY=your_firebase_api_key
FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
FIREBASE_PROJECT_ID=your_firebase_project_id
```

### 4. Run the Development Server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 5. Build for Production
```bash
npm run build
npm start
```

---

## 🖥️ Usage

### Standalone HTML Demo
Simply open `index.html` in any modern browser — no server required. The landing page is fully self-contained with all styles and scripts inline.

### Generating a Business Idea
1. Navigate to the **Hero** section
2. Click **⚡ Generate Business Idea**
3. Enter a text prompt (or upload a voice note / image / document)
4. The AI pipeline processes your input through IBM Orchestrate agents
5. Receive a structured output including:
   - Business concept & problem statement
   - Target audience & revenue models
   - Market opportunity (TAM / SAM / SOM)
   - SWOT analysis
   - Innovation score (1–10)
   - Implementation roadmap

### Light / Dark Mode Toggle
- Click the **🌙 / ☀️ toggle** in the top navigation bar
- Your preference is saved automatically in `localStorage`

---

## 🌐 Supported Industries

The Agentic AI monitors trends across 18+ domains:

`🤖 AI/ML` · `🏥 Healthcare` · `🌱 Sustainability` · `📚 EdTech` · `🌾 AgriTech` · `💰 FinTech` · `🏙️ Smart Cities` · `📡 IoT` · `🤖 Robotics` · `🛒 E-Commerce` · `🚗 Mobility` · `🔐 Cybersecurity` · `🏗️ Construction Tech` · `🎮 Gaming & Metaverse` · `✈️ Travel` · `⚡ Energy Tech` · `🧬 Biotech` · `🎯 Future of Work`

---

## 🤖 Agentic AI Architecture

```
User Input (text / voice / image / doc)
         │
         ▼
  ┌─────────────────┐
  │  IBM watsonx.ai  │  ← IBM Granite model parses intent & context
  └────────┬────────┘
           │
           ▼
  ┌─────────────────────────────────────────┐
  │         IBM Orchestrate (Multi-Agent)    │
  │                                         │
  │  ┌──────────────┐  ┌──────────────────┐ │
  │  │ Research Agent│  │ Market Agent     │ │
  │  │ (papers/news) │  │ (trends/TAM/SAM) │ │
  │  └──────────────┘  └──────────────────┘ │
  │                                         │
  │  ┌──────────────┐  ┌──────────────────┐ │
  │  │ Scoring Agent │  │ Synthesis Agent  │ │
  │  │ (feasibility) │  │ (final output)   │ │
  │  └──────────────┘  └──────────────────┘ │
  └─────────────────────────────────────────┘
           │
           ▼
  ┌─────────────────┐
  │  IBM Langflow    │  ← Visual pipeline for structured output formatting
  └────────┬────────┘
           │
           ▼
  Structured Business Idea Output
  (concept · SWOT · roadmap · score · canvas)
```

---

## 📊 Output Structure

Each generated business idea includes:

```json
{
  "title": "AI-Powered Medical Diagnosis for Rural Areas",
  "problem": "Limited access to specialist diagnosis in rural regions",
  "solution": "Mobile-first AI triage and diagnosis tool using IBM Granite",
  "targetAudience": ["Rural clinics", "NGOs", "Government health programmes"],
  "revenueModels": ["SaaS subscription", "Per-diagnosis API fee", "Government contracts"],
  "marketOpportunity": {
    "TAM": "$2.1B",
    "SAM": "$580M",
    "SOM": "$340M"
  },
  "swot": {
    "strengths": ["First-mover in rural AI health", "Low cost delivery"],
    "weaknesses": ["Connectivity dependency", "Regulatory approval time"],
    "opportunities": ["Government digital health initiatives", "NGO partnerships"],
    "threats": ["Incumbent telemedicine players", "Data privacy regulations"]
  },
  "innovationScore": 9.4,
  "feasibilityScore": 87,
  "roadmap": ["MVP in 3 months", "Pilot with 10 clinics at 6 months", "Scale to 3 states at 12 months"],
  "industry": "Healthcare"
}
```

---

## 🏆 IBM Hackathon Compliance

This project satisfies all mandatory IBM technology requirements:

- ✅ **IBM watsonx.ai** — Core AI runtime powering all language generation
- ✅ **IBM Granite Models** — Foundation model for business reasoning and output
- ✅ **IBM Langflow** — Visual workflow pipelines for multi-step AI orchestration
- ✅ **IBM Orchestrate** — Embedded chat widget + multi-agent automation layer

---

## 📄 License

This project is built for the **IBM Hackathon 2025** Innovation Showcase.

---

## 👥 Team

Built with ❤️ for the IBM Hackathon 2025 — demonstrating the power of Agentic AI and IBM watsonx for real-world business innovation.

---

*Made with IBM Bob*
