# Upload Instructions

The following files from `C:\Users\brjul\OneDrive\Documents\Projects\ClaudePPT` need to be uploaded manually:

## Binary Files Requiring Manual Upload

Due to GitHub API limitations for binary files, please upload these files directly through the GitHub web interface or using Git command line:

### PowerPoint Files
1. **Canva Design.pptx** (~10MB)
   - Professional presentation template with modern blue design
   
2. **MCP_Security_Report.pptx** (~54KB)
   - Comprehensive security presentation on Model Context Protocol

### PDF File
3. **MCP_Security_Report.pdf** (~110KB)
   - PDF version of the MCP security presentation

### Image File
4. **NotebookLM Mind Map.png** (~2.2MB)
   - Visual mind map of MCP concepts

### Video File (Requires Git LFS)
5. **NotebookLM - MCP__AI_s_Double-Edged_Sword.mp4** (~26MB)
   - Video presentation about MCP security
   - **Note**: This file exceeds standard GitHub limits. Use Git LFS for this file.

### Large Document
6. **Comprehensive Report on MCP and Associated Security Risks.md** (326 lines)
   - Detailed report with 45 citations on MCP security
   - Place in `/docs/` directory

## How to Upload

### Option 1: GitHub Web Interface
1. Go to https://github.com/bjulius/ClaudePPTX
2. Click "Add file" → "Upload files"
3. Drag and drop the files (except the video)
4. Commit the changes

### Option 2: Git Command Line
```bash
# Clone the repository
git clone https://github.com/bjulius/ClaudePPTX.git
cd ClaudePPTX

# For the video file, set up Git LFS first
git lfs track "*.mp4"
git add .gitattributes

# Copy all files to the repository
# Then add and commit
git add .
git commit -m "Add presentations and documentation"
git push origin main
```

## Repository Structure

```
ClaudePPTX/
├── README.md
├── docs/
│   ├── Design_Elements_of_Canva_Template.md ✅ (uploaded)
│   └── Comprehensive_Report_on_MCP_and_Associated_Security_Risks.md (to upload)
├── presentations/
│   ├── Canva_Design.pptx (to upload)
│   └── MCP_Security_Report.pptx (to upload)
├── pdfs/
│   └── MCP_Security_Report.pdf (to upload)
├── media/
│   ├── NotebookLM_Mind_Map.png (to upload)
│   └── NotebookLM_MCP_AI_Double_Edged_Sword.mp4 (to upload via LFS)
└── UPLOAD_INSTRUCTIONS.md ✅ (this file)
```