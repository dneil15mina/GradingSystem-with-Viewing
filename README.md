# Free k12 Grading System 
**DepEd-Aligned K12 Grading System with AI Integration**  
*(For Philippine Schools and Academic Institutions)*  

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PHP Version](https://img.shields.io/badge/PHP-8.1%2B-blue.svg)](https://www.php.net/)
[![DepEd Compliance](https://img.shields.io/badge/DepEd%20Compliance-DO%208%2C%20s.2015-green)](https://www.deped.gov.ph/wp-content/uploads/2015/04/DO_s2015_08.pdf)

![System Preview]

## 📌 Key Features  
**Philippine Education Focused**  
✅ **Per-Level Composite Views**  
- Grade 1-12 academic summaries  
- Senior High track comparisons (STEM, ABM, HUMSS, TVL)  

✅ **DepEd-Compliant Calculations**  
- Transmutation formulas from DepEd Order No. 8  
- Automated SF9/SF10 report generation  

✅ **Multi-Role Access**  
- Admin: Complete system control  
- Teachers: Grade encoding portal  
- Students/Parents: Mobile-friendly grade viewing  
- Academic Coordinators: School-wide analytics  

✅ **PH Data Privacy Act Ready**  
- NPC Circular 16-03 compliant security  
- Automatic data anonymization for exports  

✅ **AI-Powered Insights**  
- DeepSeek R1 integration for predictive analytics  

## 🚀 Installation  

### Requirements  
- PHP 8.1+ (with `gd` and `pdo_sqlite` extensions)  
- Node.js 18+ (for AI features)  
- Composer (Dependency Manager)  

### Quick Start  
```bash
# Clone repository
git clone https://github.com/dneil15mina/GradingSystem-with-Viewing
cd academictrack-pro

# Install PHP dependencies
composer install

# Install Node.js modules
npm install

# Initialize configuration 
cp .env.example .env
```

## 🔧 Configuration  
1. **Environment Setup**  
```ini
# .env
DB_CONNECTION=sqlite
DB_DATABASE=/var/www/data/k12_grades.db

SCHOOL_REGION=PH-NCR  # PH region code
```

2. **Database Initialization**  
```bash
php artisan migrate --seed
```

3. **AI Services Setup**  
```bash
npm run ai:configure
```

## 🧑💻 Usage Examples  

### Grade Calculation (DepEd Formula)  
```javascript
// Calculate final grade using DepEd weights
function calculateFinalGrade(ww, pt, qa) {
  return (ww * 0.3) + (pt * 0.5) + (qa * 0.2);
}
```
```

## 📱 Mobile Optimization  
```css
/* Mobile-first grade cards */
@media (max-width: 768px) {
  .grade-card {
    flex-direction: column;
    padding: 1rem;
  }
  
  .ph-data-table {
    overflow-x: auto;
  }
}
```

## 📅 Roadmap  
- [ ] Mobile app (React Native)  
- [ ] Integration with DepEd LMS  
- [ ] AI-powered grade predictions (Q2 2025)  
- [ ] Regional division benchmarking  

## 📜 License  
MIT License - See [LICENSE](LICENSE)  

---

 (How to Contribute)  
Mag-email sa [admin@smarterjuan.org](mailto:admin@smarterjuan.org)

*This project adheres to DepEd's Open Source Initiative for Philippine Education.*
```

---

### Recommended Repository Structure  
```bash
.
├── public/              # Web root
│   ├── css/             # PH school-branded styles
│   └── js/              # Vanilla JS modules
├── src/
│   ├── PH/              # Philippine-specific classes
│   │   ├── DepEdCalculator.php
│   │   └── DataPrivacyHelper.php
│   └── AI/              # AI integration
├── docs/
│   ├── deped-compliance.md
│   └── screenshots/     # PH UI previews
├── database/
│   └── schemas/         # K12 database design
└── tests/
    └── PH/              # Philippine test cases
```

---

### Key PH-Specific Elements to Highlight  
1. **DepEd Compliance Badges**  
   - Official DepEd memo references  
   - NPC data privacy certification status  

2. **Regional Configuration**  
   - PH region code system (e.g., PH-NCR, PH-REGIONVII)  
   - Local holiday calendar integration  

3. **Filipino Language Support**  
   - Tagalog UI translations  
   - Mixed English-Filipino documentation  

4. **PH Deployment Guide**  
   ```markdown
   ## 🇵🇭 PH Hosting Recommendations
   - **Preferred Providers**: HostKoala PH, Dews.IO
   - **Required**: PH-based SSL certificates
   - **Optimization**: Configure for Globe/Smart mobile networks
   ```

