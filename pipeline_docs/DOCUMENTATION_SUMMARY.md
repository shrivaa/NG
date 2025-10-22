# Pipeline Documentation Package

## 📦 Package Contents

This comprehensive documentation package contains everything you need to understand, use, and maintain the N. gonorrhoeae Outbreak Analysis Pipeline.

### Documentation Files

| File | Description | Size |
|------|-------------|------|
| **index.html** | Main overview with pipeline statistics, navigation hub | 15 KB |
| **process_flow.html** | Step-by-step workflow execution with QC checkpoints | 54 KB |
| **data_flow.html** | Sample tracking, data transformations, caching logic | 26 KB |
| **flowcharts.html** | Interactive Mermaid diagrams (high-level + detailed) | 23 KB |
| **module_reference.html** | Complete process documentation (60+ modules) | 61 KB |
| **README.txt** | Quick start guide | 1 KB |

**Total Documentation Size:** ~188 KB

---

## 🎯 What's Documented

### Pipeline Coverage
- ✅ **14 Workflows** fully documented
- ✅ **60+ Modules** with detailed specifications
- ✅ **9 Analysis Types** (QC, Assembly, AMR, Phylogeny, etc.)
- ✅ **3 QC Stages** with filtering logic
- ✅ **3 Caching Systems** for performance optimization

### Documentation Depth

#### 1. Process Flow Documentation
- **10 Major Steps** with substeps
- Decision points at each stage
- QC checkpoint descriptions
- Input/output specifications
- Conditional workflow execution
- Parameter documentation

#### 2. Visual Flowcharts
- High-level pipeline overview
- QC workflow details (QC1 & QC2)
- Assembly smart caching logic
- Variant calling with cache filtering
- AMR profiler (chromosomal + HGT)
- Advanced analysis workflows
- Color-coded by workflow type

#### 3. Data Flow Documentation
- Channel structure and formats
- Sample tracking through pipeline
- Filtering impact analysis
- Three-tier caching system
- Data transformation diagrams
- Output file organization
- Data provenance tracking

#### 4. Module Reference
- Process purpose and description
- Input/output specifications
- Container information
- Parameters with defaults
- Usage examples
- Notes and best practices
- Organized by 15 categories

---

## 🚀 Quick Start

1. **Open** `index.html` in your web browser
2. **Navigate** using the colorful cards on the main page
3. **Explore** workflows, data flow, or specific modules
4. **Search** (Ctrl+F) for specific terms or processes

### Recommended Reading Order

For new users:
1. Start with **index.html** for overview
2. Read **process_flow.html** for execution sequence
3. Check **flowcharts.html** for visual understanding
4. Reference **module_reference.html** for specific details
5. Consult **data_flow.html** for caching/tracking

For experienced users:
- Jump directly to **module_reference.html** for quick lookups
- Use **flowcharts.html** for visual workflow reminders
- Check **data_flow.html** for caching behavior

---

## 📊 Pipeline Statistics

### Workflow Organization
| Category | Count | Purpose |
|----------|-------|---------|
| Sample Discovery & QC | 2 | Input cataloging, species verification |
| Reads QC | 4 | FastP filtering, QC1 checks |
| Assembly | 5 | SPAdes assembly, caching, stats |
| Assembly QC | 5 | Coverage, QC2 comprehensive filtering |
| Downsampling | 3 | Read normalization |
| Variant Calling | 8 | Snippy, Gubbins, core alignment |
| MLST Analysis | 4 | Sequence typing, clustering |
| AMR Typing | 2 | NG-MAST/NG-STAR |
| AMR Chromosomal | 7 | Mutation detection, alleles |
| AMR HGT | 4 | HGT gene presence/absence |
| Clinical | 4 | Treatment recommendations |
| Phylogeny | 4 | RAxML-NG, visualization |
| Outbreak | 2 | SNP distance clustering |
| Recombination | 2 | Functional annotation |
| Reporting | 4 | Manifest generation |
| **TOTAL** | **60** | **modules** |

### Analysis Capabilities
- **Quality Control:** 3 stages (discovery, reads, assembly)
- **Assembly:** SPAdes with smart caching
- **Variant Calling:** Snippy + Gubbins recombination removal
- **Phylogenetics:** RAxML-NG with bootstrap
- **Outbreak Detection:** SNP-based clustering
- **AMR Profiling:** Chromosomal mutations + HGT genes
- **Typing:** MLST, NG-MAST, NG-STAR, cgMLST
- **Clinical Interpretation:** Treatment recommendations (planned)

---

## 🎨 Documentation Features

### Interactive Elements
- ✨ Mermaid flowcharts (render in browser)
- 🔗 Internal navigation links
- 📋 Collapsible sections
- 🎨 Color-coded workflows
- 📊 Data tables for quick reference
- 💡 Highlighted notes and warnings

### Visual Design
- Clean, professional styling
- Consistent color scheme (purple/blue gradient)
- Responsive layout
- Easy-to-read typography
- Icon-based navigation
- Sticky headers for easy access

### Content Organization
- Hierarchical structure
- Step-by-step instructions
- Decision trees clearly marked
- QC checkpoints highlighted
- Container badges for each process
- Parameter lists with defaults

---

## 🔍 Key Concepts Explained

### Quality Control Strategy
The pipeline implements a "fail-forward" approach:
- **QC1 (Reads):** FastP-based filtering - failures stop here
- **QC2 (Assembly):** Comprehensive filtering - failures continue selectively
- **All samples** tracked in manifests for transparency

### Caching Intelligence
Three-tier caching system:
1. **Assembly Cache:** Avoid re-assembling unchanged samples
2. **Snippy Core Cache:** Reuse variant calling (with smart exclusions)
3. **AMR Snippy Cache:** Reuse resistance analysis

### Sample Flow
```
100 samples discovered
↓
95 pass QC1 (reads quality)
↓
85 pass QC2 (assembly quality)
↓
Expensive analyses (phylogeny, outbreak)
+
10 QC2-failed → Typing/AMR only
+
5 QC1-failed → Logged in reports
```

---

## 📝 Using This Documentation

### For Pipeline Users
- Learn workflow execution order
- Understand QC filtering criteria
- Configure caching for performance
- Interpret output file structure
- Troubleshoot issues

### For Pipeline Developers
- Understand module dependencies
- Modify workflows safely
- Add new analysis modules
- Debug data flow issues
- Maintain code quality

### For Bioinformaticians
- Understand analysis rationale
- Evaluate result quality
- Customize parameters
- Integrate with other tools
- Validate findings

---

## 🔧 Technical Details

### Requirements for Viewing
- Modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled (for Mermaid diagrams)
- No server required - open HTML files directly

### File Formats
- **HTML5** with CSS3 styling
- **Mermaid.js** for flowcharts (CDN-loaded)
- **JSON** for module inventory
- **Markdown** for README files

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

---

## 📄 License & Copyright

**Copyright © 2025 I Graviton, LLC**  
All rights reserved.

This documentation is provided for use with the N. gonorrhoeae Outbreak Analysis Pipeline.

---

## 📞 Support & Feedback

For questions about this documentation or the pipeline:
1. Check the relevant documentation section first
2. Search for specific terms using browser find (Ctrl+F)
3. Review the flowcharts for visual understanding
4. Consult the module reference for technical details

---

## 🎉 Documentation Complete!

This package represents comprehensive documentation of:
- **14 workflows** across the entire pipeline
- **60+ processes** with full specifications  
- **All data flows** from input to output
- **Complete caching logic** for performance
- **Visual diagrams** for quick understanding

**Happy analyzing! 🧬**

---

*Generated: October 22, 2025*  
*Pipeline Version: Based on current Nextflow implementation*  
*Documentation Format: HTML5 + Mermaid.js + Markdown*
