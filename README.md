[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18849987.svg)](https://doi.org/10.5281/zenodo.18849987)
# 📝 LexiNegotiate

> AI-Powered Contract Analysis & Negotiation Assistant

**Democratizing legal protection for 800 million freelancers worldwide** — putting a $300/hr lawyer in their pocket, powered by Google Gemini.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Node Version](https://img.shields.io/badge/node-%3E%3D20.0.0-brightgreen)](https://nodejs.org)
[![React](https://img.shields.io/badge/react-19.2.4-61DAFB?logo=react)](https://reactjs.org)
[![Google Gemini](https://img.shields.io/badge/Gemini-3.0-4285F4?logo=google)](https://ai.google.dev)

---

## 🎯 The Problem

Most freelancers and small business owners sign contracts blindly because they cannot afford the **$300/hour legal fees** for professional review. A single "simple" agreement with unlimited liability can lead to catastrophic losses — like a colleague who lost **$50,000 in legal fees** over a single software bug.

**LexiNegotiate** was built to turn legal jargon into actionable financial data and empower users to negotiate with confidence.

---

## ✨ Key Features

### 🎯 **Instant Risk Assessment**
- Analyzes contracts in seconds via PDF upload, image scan, or text paste
- Generates a **0-100 risk score** with color-coded severity levels
- Identifies predatory clauses and legal traps

### 💰 **Financial Impact Calculator**
- Quantifies exact monetary exposure (e.g., uncapped late fees, unlimited liability)
- Shows **total potential exposure** and **negotiable savings**
- Breaks down immediate risk, annual exposure, and lifetime cost

### 🤝 **3-Tier Negotiation Strategy**
- **Tier 1 (Ideal)**: Your best-case scenario with strong legal backing
- **Tier 2 (Compromise)**: Balanced middle ground with sweeteners
- **Tier 3 (Minimum)**: Your walk-away threshold
- Context-aware scripts for each tier

### 💬 **AI Negotiation Mentor**
- Real-time context-aware chat coach powered by Gemini
- Roleplay difficult conversations before they happen
- Get specific legal references (French Code Civil, SYNTEC framework)
- Suggested action buttons for quick follow-ups

### 🎙️ **Audio Coaching (TTS)**
- Built-in Text-to-Speech using Gemini Flash TTS
- "Hear the Script" feature to practice negotiation delivery
- Professional voice generation for realistic preparation

### 📊 **Visual Comparison Editor**
- Side-by-side comparison: Original vs. Amended clauses
- Color-coded change summary (deleted/added/clarified)
- Financial protection breakdown per clause
- Export to PDF for professional presentation

### 📧 **Email Draft Generator**
- Three tone options: Formal, Professional-Friendly, Collaborative
- Pre-filled subject lines and body text
- One-click Gmail/Outlook integration
- Templates based on successful negotiations

### 📈 **Success Stories & Statistics**
- Community-sourced negotiation outcomes (simulated for demo)
- Success rate percentages and average resolution times
- Winning arguments and common concerns database

---

## 🛠️ Technology Stack

### **Frontend**
- **React 19** with TypeScript for type-safe development
- **Tailwind CSS** for responsive, production-grade UI design
- **Vite** for lightning-fast build and HMR (Hot Module Replacement)

### **AI & Intelligence**
- **Google Gemini 3.0 Pro** (32K thinking budget) for deep contract reasoning
- **Gemini Vision** (Multimodal) for OCR from photos and PDFs with 98%+ accuracy
- **Gemini Flash** for low-latency chat and real-time responses
- **Gemini Flash TTS** for professional audio generation

### **Architecture**
- Stateless, privacy-first design (no data storage)
- Client-side processing for maximum security
- TypeScript interfaces for legal and financial domain modeling
- Structured JSON output with strict schema validation

---

## 🚀 Quick Start

### **Prerequisites**
- Node.js >= 20.0.0
- npm or yarn
- Google Gemini API key

### **Installation**

1. **Clone the repository**
```bash
git clone https://github.com/hafididrissi/lexinegotiate.git
cd lexinegotiate
```

2. **Install dependencies**
```bash
npm install
```

3. **Configure environment**
Create a `.env.local` file in the root directory:
```env
GEMINI_API_KEY=your_api_key_here
```

> 🔑 **Get your API key**: Visit [Google AI Studio](https://aistudio.google.com/app/apikey)

4. **Launch development server**
```bash
npm run dev
```

5. **Open in browser**
Navigate to `http://localhost:3000`

### **Production Build**
```bash
npm run build
npm run preview
```

---

## 📖 Usage Guide

### **1. Upload Your Contract**
- **Option A**: Paste text directly into the input field
- **Option B**: Upload a PDF or image (photo of printed contract)
- Supports multiple formats: .pdf, .jpg, .png, .jpeg

### **2. AI Analysis**
LexiNegotiate automatically:
- Extracts all clauses and legal terms
- Identifies risks (HIGH/MEDIUM/LOW)
- Calculates financial exposure
- Generates negotiation strategies

### **3. Review Results**
- **Risk Gauge**: Overall contract safety score (0-100)
- **Financial Summary**: Total exposure vs. potential savings
- **Clause Breakdown**: Detailed analysis of each problematic term
- **Negotiability Score**: How likely each change is to be accepted

### **4. Negotiate with Confidence**
For each risky clause:
- Read the simplified explanation
- Review the 3-tier negotiation strategy
- Use the "Hear Script" button to practice
- Generate professional email drafts
- Access success stories for confidence

### **5. Export & Share**
- Export analysis as PDF (print or save)
- Share via native share API or clipboard
- Send drafted emails directly via Gmail/Outlook

---

## 🏗️ Project Structure

```
lexinegotiate/
├── components/              # React components
│   ├── ClauseCard.tsx      # Individual clause display
│   ├── ComparisonModal.tsx # Visual comparison editor
│   ├── NegotiationChat.tsx # AI mentor chatbot
│   └── RiskGauge.tsx       # Risk score visualization
├── services/
│   └── geminiService.ts    # Gemini API integration
├── types.ts                # TypeScript interfaces
├── App.tsx                 # Main application component
├── index.tsx               # React entry point
├── vite.config.ts          # Vite configuration
└── package.json            # Dependencies
```

---

## 🔒 Privacy & Security

- **No Data Storage**: All processing happens client-side
- **Stateless Architecture**: Contracts are not saved or logged
- **API Key Protection**: Environment variables for sensitive credentials
- **HTTPS Only**: Secure communication with Gemini API

> ⚠️ **Never commit** your `.env` or `.env.local` files to version control. They are listed in `.gitignore` for your protection.

---

## 🎨 Key Design Principles

1. **User-Centric**: Legal jargon translated to plain language
2. **Actionable**: Every insight includes concrete next steps
3. **Empowering**: Confidence-building through preparation
4. **Transparent**: Clear financial calculations with no hidden assumptions
5. **Accessible**: Mobile-responsive, print-friendly, keyboard navigable

---

## 🌍 Target Audience

- **Freelancers & Contractors**: Web developers, designers, consultants
- **Small Business Owners**: Entrepreneurs, startups, sole proprietors
- **Students & Interns**: First-time contract signers
- **Anyone**: Who needs affordable legal protection

**Geographic Focus**: Built with French legal standards (Code Civil, SYNTEC) but adaptable to other jurisdictions.

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Report bugs** via [GitHub Issues](https://github.com/hafididrissi/lexinegotiate/issues)
2. **Suggest features** or improvements
3. **Submit pull requests** for bug fixes or enhancements
4. **Improve documentation** for clarity and completeness

### Development Guidelines
- Follow TypeScript best practices
- Maintain Tailwind CSS conventions
- Add tests for new features (coming soon)
- Update documentation for API changes

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Hafid Idrissi**  
Fullstack DevOps Engineer specializing in Cloud Architecture, AI Integration, and Scalable SaaS.

- GitHub: [@hafididrissi](https://github.com/hafididrissi)
- LinkedIn: [Hafid Idrissi](https://linkedin.com/in/hafid-idrissi)

---

## 🏆 Built For

**Google Gemini 3 Hackathon 2026**

Developed with ❤️ to empower freelancers worldwide with accessible legal intelligence.

---

## 🙏 Acknowledgments

- **Google Gemini Team** for the incredible AI capabilities
- **React & Vite Communities** for excellent tooling
- **Freelance Community** for inspiration and feedback
- **Legal Experts** who helped validate the approach

---

## 📞 Support

- **Documentation**: This README and inline code comments
- **Issues**: [GitHub Issues](https://github.com/HafidIdrissi/LexiNegotiate-/issues)
- **Discussions**: [GitHub Discussions](https://github.com/hafididrissi/lexinegotiate-/discussions)

---

## 🗺️ Roadmap

### Phase 1 (Current - Hackathon Demo)
- ✅ Core contract analysis engine
- ✅ Financial impact calculator
- ✅ 3-tier negotiation strategy
- ✅ AI mentor chatbot
- ✅ Audio coaching (TTS)

### Phase 2 (Post-Hackathon)
- [ ] Multi-language support (English, Spanish, German)
- [ ] Real user database for success stories
- [ ] Contract template library (SYNTEC, NDA, SLA)
- [ ] Browser extension for inline analysis
- [ ] Mobile app (React Native)

### Phase 3 (Future)
- [ ] Collaborative negotiation (multi-party contracts)
- [ ] Integration with e-signature platforms
- [ ] Legal expert verification network
- [ ] Enterprise version with team features

---

## ⚖️ Legal Disclaimer

**LexiNegotiate is an AI-powered assistant tool, not a licensed attorney.**

- This software provides information and suggestions, not legal advice
- Always consult a qualified lawyer for binding legal opinions
- Use at your own risk and judgment
- The creators assume no liability for decisions made based on this tool

**For critical contracts** (>€50,000 value, complex IP, or high-stakes agreements), we recommend professional legal review in addition to using LexiNegotiate.

---

<div align="center">

**Made with 🤖 Gemini, ⚛️ React, and ❤️ for Freelancers**

[Report Bug](https://github.com/hafididrissi/lexinegotiate-/issues) · [Request Feature](https://github.com/hafididrissi/lexinegotiate-/issues) · [Documentation](https://github.com/hafididrissi/lexinegotiate-/wiki)

</div>
