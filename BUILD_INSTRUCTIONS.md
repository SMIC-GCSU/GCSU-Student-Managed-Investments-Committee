# Building SMIC Portfolio Analysis Executables

## Prerequisites

- Python 3.10 or higher
- All dependencies from `requirements.txt`
- PyInstaller: `pip install pyinstaller`

## Windows Build

Run the build script:
```bash
build_windows.bat
```

Or manually:
```bash
pyinstaller SMIC_Portfolio_Analysis.spec --clean
```

The executable will be in `dist/SMIC_Portfolio_Analysis.exe`

## macOS Build

Run the build script:
```bash
./build_macos.sh
```

Or manually:
```bash
python3 -m PyInstaller SMIC_Portfolio_Analysis_macos.spec --clean
cd dist
zip -r SMIC_Portfolio_Analysis_macos.zip "SMIC Portfolio Analysis.app"
```

## Included in Distribution

- Application executable/bundle
- All Python dependencies
- `data/transactions.csv` file
- Publisher metadata: Joel Saucedo - GCSU SMIC Managing Director
- Copyright: Copyright (C) 2024-2025 Joel Saucedo, GCSU Student Managed Investment Committee

## Creating a Release

1. Tag the release: `git tag v1.0.0`
2. Push the tag: `git push origin v1.0.0`
3. GitHub Actions will automatically build and create a release
4. Download links will be available on the landing page

