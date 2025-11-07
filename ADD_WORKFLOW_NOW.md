# ⚡ ADD WORKFLOW NOW TO BUILD EXECUTABLES

## Quick Steps (2 minutes)

### Step 1: Add Workflow File to GitHub

1. **Open this URL in your browser:**
   ```
   https://github.com/SMIC-GCSU/portfolio/new/main?filename=.github/workflows/build-release.yml
   ```

2. **Copy the ENTIRE content from this file:**
   - File: `.github/workflows/build-release.yml` (in your local repo)
   - Or see: `WORKFLOW_FILE_CONTENT.txt`

3. **Paste into the GitHub editor**

4. **Click "Commit new file"**

### Step 2: Push the Tag (This Triggers the Build!)

```bash
git push origin v1.0.0
```

**That's it!** GitHub Actions will automatically:
- ✅ Build Windows .exe
- ✅ Build macOS .app  
- ✅ Create GitHub Release
- ✅ Upload both files

### Step 3: Check Build Status

Visit: https://github.com/SMIC-GCSU/portfolio/actions

The build will take about 10-15 minutes. Once complete, downloads will be available at:
- https://smic-gcsu.github.io/
- https://github.com/SMIC-GCSU/portfolio/releases

## What Gets Built

- **Windows:** `SMIC_Portfolio_Analysis.exe` (includes transaction.csv)
- **macOS:** `SMIC_Portfolio_Analysis_macos.zip` (includes transaction.csv)
- **Publisher:** Joel Saucedo - GCSU SMIC Managing Director
- **Copyright:** Copyright (C) 2024-2025 Joel Saucedo, GCSU SMIC

