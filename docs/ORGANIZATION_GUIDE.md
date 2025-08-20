# Tissue Dynamics GitHub Organization

## 🧬 Welcome to Tissue Dynamics

We are pioneering the future of drug discovery and tissue engineering through innovative organoid technology and advanced computational analysis. Our repositories contain the tools, analyses, and infrastructure that power our research and development efforts.

## 🏗️ Repository Architecture

### Core Infrastructure
- **td-ui** - Shared UI component library for all Tissue Dynamics applications
- **deployment** - Production deployment and data processing pipelines
- **td-lab** - Laboratory information management system

### Applications
- **402-rna-app** - RNA-seq data management and analysis platform
- **organoid-detection-tool** - Desktop application for organoid image analysis
- **deep-researcher** - AI-powered research assistant for PK values and clinical data
- **pk-database-automation** - Automated pharmacokinetic database population

### Research & Analysis
- **td-aging-rnaseq** - Aging-related RNA-seq analysis
- **402-sanofi-rnaseq** - Sanofi collaboration RNA-seq analysis
- **402-oddity-skin-aging** - Skin aging target identification
- **402-ubl5-data** - UBL5 data exploration

### Papers & Publications
- **hu-ht-paper** - High-throughput toxicity prediction paper
- **hu-toxicity-paper-v2** - Improved toxicity prediction methodology
- **td-smiles-based-liver-tox** - SMILES-based liver toxicity ML/DL models
- **td-structural-toxicity-prediction** - Molecular encoding methods comparison

### Experimental & Archives
- **organospheres-research** - Organosphere research experiments
- **organoid-embedding-experiments** - Embedding methods for oxygen time series
- **402-pilot-liver-panel** - qPCR liver panel experiments

## 📋 Repository Naming Conventions

### Prefix Standards
Use prefixes to indicate project origin and affiliation:

#### **td-** prefix (Standard)
The primary prefix for Tissue Dynamics projects:
- `td-rna` - RNA-seq analysis platform
- `td-ui` - UI component library
- `td-lab` - Laboratory management system
- `td-aging-rnaseq` - Aging research analysis

#### **402-** prefix (Legacy - Shaun's early work)
Projects created during the 402 early period:
- `402-rna-app` - RNA application (consider renaming to td-rna)
- `402-bpiq-explorer` - Data exploration tool
- `402-cloud-manager` - Cloud infrastructure
- `402-sanofi-rnaseq` - Sanofi collaboration

#### **hu-** prefix (Hebrew University affiliation)
Projects with Hebrew University collaboration:
- `hu-ht-paper` - Hebrew University high-throughput studies
- `hu-toxicity-paper` - Hebrew University toxicity research

#### **dynamix-** prefix
Projects specifically for the Dynamix machine:
- `dynamix-insights` - Dynamix data insights
- `dynamix-switcher-patch` - Dynamix system patches
- `td-dynamix-toolbox` - Dynamix analysis tools
- `td-dynamix-desktop` - Dynamix desktop application

#### **os-** prefix (Organospheres)
Organosphere-specific projects:
- `organospheres` - Main organosphere repository
- `organospheres-research` - Organosphere research
- `organospheres-detection-tool` - Organosphere detection
(Note: Some use full "organospheres" without prefix)

### Repository Categories

#### 🔬 **Research Repositories**
Format: `{prefix}-{topic}-{subtype}`
- `td-aging-rnaseq`
- `402-sanofi-rnaseq`
- `402-oddity-skin-aging`

#### 🛠️ **Tool Repositories**
Format: `{prefix}-{tool-name}`
- `organoid-detection-tool`
- `402-bpiq-explorer`
- `402-data-editor`

#### 📊 **Data Analysis**
Format: `{prefix}-{dataset}-{analysis}`
- `402-ubl5-data`
- `402-pilot-liver-panel`

#### 📄 **Papers/Publications**
Format: `{author/collab}-{topic}-paper`
- `hu-toxicity-paper`
- `hu-ht-paper`

#### 🏗️ **Infrastructure**
Clear, descriptive names:
- `deployment`
- `402-cloud-manager`
- `402-cf-secrets-sync`

## 🚀 Best Practices

### Repository Setup
1. **Always include a README** with:
   - Purpose and overview
   - Installation instructions
   - Usage examples
   - Contact information

2. **Use descriptive names**:
   - ✅ `402-rna-app` (clear purpose)
   - ❌ `General` (too vague)

3. **Add meaningful descriptions** in GitHub settings

4. **Include appropriate .gitignore** for your tech stack

5. **Set up branch protection** for main/master branches

### Code Organization
```
repository/
├── README.md           # Project overview
├── CLAUDE.md          # AI assistant instructions
├── docs/              # Documentation
├── src/               # Source code
├── tests/             # Test files
├── scripts/           # Utility scripts
└── Sandbox/           # Experimental code
```

### Security
- **Never commit secrets** - Use environment variables
- **Keep sensitive repos private** until ready for publication
- **Use Cloudflare Secrets** for production credentials
- **Implement proper access controls** in applications

### Collaboration
1. **Use clear commit messages**:
   ```
   feat: Add RNA-seq normalization module
   fix: Correct batch effect in PCA analysis
   docs: Update installation instructions
   ```

2. **Create issues** for bugs and feature requests

3. **Use pull requests** for code review

4. **Tag releases** for production deployments

## 🔄 Migration Guide

### Renaming Recommendations
To align with our naming conventions:

#### Consider Renaming (402 → td):
Since `td-` is the standard prefix and `402-` was early experimental work:
- `402-rna-app` → Keep as `td-rna` (already created)
- `402-cloud-manager` → `td-cloud-manager`
- `402-data-editor` → `td-data-editor` (or archive if not used)
- `402-bpiq-explorer` → `td-bpiq-explorer`

#### Keep As-Is:
- **td-** prefixed repos (already following standard)
- **hu-** prefixed repos (indicates Hebrew University collaboration)
- **dynamix-** prefixed repos (machine-specific)
- **organospheres** repos (domain-specific)

### Renaming Process

1. **Safe to rename** (minimal dependencies):
   - Standalone analysis repos
   - Internal tools
   - Documentation repos
   - Most 402- prefixed repos

2. **Requires coordination** (has dependencies):
   - `td-ui` (npm package - DO NOT rename)
   - `deployment` (CI/CD pipelines)
   - Any repo with webhooks or external integrations

3. **Steps for renaming**:
   ```bash
   # Update local remote
   git remote set-url origin https://github.com/Tissue-Dynamics/new-name
   
   # Update package.json if applicable
   # Update CI/CD configurations
   # Notify team members
   # Update any documentation references
   ```

## 📚 Key Technologies

- **Frontend**: SvelteKit, React, Svelte 5
- **Backend**: Cloudflare Workers, Node.js, Python
- **Databases**: Cloudflare D1, PostgreSQL, R2 Storage
- **ML/AI**: PyTorch, scikit-learn, Claude API
- **Analysis**: R, Python (pandas, numpy, scipy)
- **Infrastructure**: AWS, Cloudflare, GitHub Actions

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📬 Contact

For questions about our repositories or collaboration opportunities:
- **GitHub Issues**: Open an issue in the relevant repository
- **General Inquiries**: Use the [General](https://github.com/Tissue-Dynamics/General) repository

## 🔒 Privacy & Compliance

Many of our repositories contain proprietary research and are private. We maintain strict access controls and follow best practices for:
- HIPAA compliance for any human data
- Laboratory data security
- Intellectual property protection

---

*Building the future of personalized medicine through organoid technology and computational biology.*