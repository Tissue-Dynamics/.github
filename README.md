# Tissue Dynamics GitHub Organization

## 🧬 Welcome to Tissue Dynamics

We are attempting to make drugs faster and cheaper for everyone. This centers around creating better disease models, engineering human tissue in the lab, automating manual biological research, and creating amazing software.

## 🏗️ Repository Architecture

### Core Infrastructure
- **td-ui** - Shared UI component library for all Tissue Dynamics applications
- **deployment** - Production deployment and data processing pipelines
- **td-lab** - Laboratory information management system
- **tissue-dynamics** - Holds code for the qc and analysis systems as well as the dynamix observability monitor

### Applications
- **402-rna-app** - RNA-seq data management and analysis platform
- **organoid-detection-tool** - Desktop application for organoid image analysis
- **deep-researcher** - AI-powered research assistant for PK values and clinical data

### Papers & Publications
- **hu-ht-paper** - High-throughput toxicity prediction paper
- **hu-toxicity-paper-v2** - Improved toxicity prediction methodology
- **td-smiles-based-liver-tox** - SMILES-based liver toxicity ML/DL models
- **td-structural-toxicity-prediction** - Molecular encoding methods comparison

## 📋 Repository Naming Conventions

### Prefix Standards
Use prefixes to indicate project origin and affiliation:

#### **td-** prefix (Standard)
The primary prefix for Tissue Dynamics projects:
- `td-rna` - RNA-seq analysis platform
- `td-ui` - UI component library
- `td-lab` - Laboratory management system
- `td-aging-rnaseq` - Aging research analysis

#### **402-** prefix (Legacy - Shaun's early/migrated work)
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
- **Use secure credential management** for production credentials
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


## 🔒 Privacy & Compliance

Many of our repositories contain proprietary research and are private. We maintain strict access controls and follow best practices for:
- HIPAA compliance for any human data
- Laboratory data security
- Intellectual property protection

---

*Building the future of personalized medicine through organoid technology and computational biology.*
