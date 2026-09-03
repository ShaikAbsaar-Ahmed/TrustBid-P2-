# TrustBid — Verify Every Bid. Trust Every Tender.

An AI-assisted compliance verification platform for government tenders — document parsing, OCR, rule matching, risk scoring and fraud detection, delivered in seconds with evidence for every decision.

## 🌟 Features

- **Smart Document Upload** - Per-type uploads with live progress and instant format validation
- **PDF Parsing + OCR** - PyMuPDF for digital text, Tesseract OCR fallback for scanned pages
- **AI Field Extraction** - Registration numbers, dates, PAN & GSTIN pulled with source-sentence evidence
- **Tender Rule Matching** - Every field checked against the tender's configurable rule set
- **Pass / Fail / Needs Review** - Three-state verdicts with uncertainty routing to human review
- **Risk Score per Bidder** - 0-100 score aggregated from rule-level risk points
- **Evidence-Based Verification** - Every verdict quotes the exact document sentence that proves it
- **Document Expiry Detection** - Automatic extraction and validation of certificate validity dates
- **Mismatch Detection** - Cross-document consistency checks (e.g., PAN card vs PAN inside GSTIN)
- **Audit Trail** - Append-only log of every upload, check and override
- **Auto Compliance Report** - One-click PDF report per bidder, plus tender-wide CSV export
- **Procurement Dashboard** - KPIs, risk bars, status chips and charts for officers
- **Role-Based Access** - Admin, officer and reviewer roles with JWT-secured permissions
- **Manual Review Override** - Officers can override any verdict with mandatory logged reason
- **Fraud Red-Flag Detection** - Specimen watermarks, duplicate file hashes, metadata anomalies

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- No backend required for demo mode

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/trustbid.git
cd trustbid
```

2. Open `trustbid.html` in your web browser:
```bash
# Simply open the HTML file in your browser
# Or use a local server:
python -m http.server 8000
# Then visit http://localhost:8000/trustbid.html
```

### Demo Mode

The current implementation includes a fully functional demo with:
- 6 sample bidder records with realistic compliance data
- Interactive dashboard with real-time updates
- AI chat assistant with pre-programmed responses
- Complete audit trail and compliance reports
- Risk scoring and fraud detection simulation

## 📊 How It Works

1. **Smart Document Upload** - Bidder certificates are uploaded per document type and stored in an encrypted, audit-locked repository
2. **AI Extraction & OCR** - PyMuPDF reads digital PDFs instantly; Tesseract OCR handles scanned pages. AI extracts registration numbers, dates, PAN & GSTIN with source-sentence evidence
3. **Rule Matching & Risk Score** - Every field is checked against the tender's rule set: expiry, cross-document consistency, verified-registry match and fraud red flags
4. **Verdict + Report** - Pass, Fail or Needs Review — with a per-bidder risk score, highlighted evidence, a downloadable compliance report and a full audit trail

## 🏗️ Architecture

### Frontend
- **HTML5** - Single-page application structure
- **CSS3** - Custom styling with dark theme and glassmorphism effects
- **JavaScript (ES6+)** - Vanilla JS for all interactivity
- **Chart.js** - Data visualization for compliance metrics

### Backend (Planned)
- **Python/Flask** - REST API for document processing
- **PyMuPDF** - PDF text extraction
- **Tesseract OCR** - Scanned document processing
- **PostgreSQL** - Secure data storage
- **JWT** - Authentication and authorization

## 🎯 Use Cases

- **Government Procurement** - Automated tender bid verification
- **Compliance Officers** - Streamlined document review process
- **Audit Trails** - Complete action history for transparency
- **Fraud Detection** - Automated red-flag identification
- **Risk Assessment** - Quantified bidder risk scoring

## 👥 Team

### Leader
- **Shaik Absaar Ahmed** - Backend APIs & Database

### Team Members
- **Mohammed Muzaffer Ali** - PDF Parsing & OCR Pipeline
- **Shaik Anas Ahmed** - Field Extraction & Rule Engine
- **Sai Jeshwanth** - Security, Reports & Testing
- **Shamitha** - Frontend Dashboard & Upload Screens
- **Sharanya** - Integration & Product Polish

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or support, please open an issue on GitHub.

---

**Built for transparent public procurement.** Compliance you can prove.