STANDALONE WINDOWS EXE BUILD PACKAGE

This package builds a single Windows x64 EXE using GitHub Actions.
The target computer does NOT need Python, pip, or PyInstaller installed.

IMPORTANT:
- This package does not contain a precompiled Windows EXE. The EXE is built
  by GitHub's Windows runner after you upload this project.
- The build computer on GitHub uses Python, but the computer running the
  finished EXE does not need Python installed.
- The application is a local Excel review tool only. It does not interact
  with the government portal, select freeze checkboxes, or freeze accounts.

BUILD STEPS:
1. Sign in to GitHub and create a new repository.
2. Upload all files/folders from this ZIP, preserving the .github/workflows/
   folder structure.
3. Open the repository's Actions tab.
4. Select "Build Standalone Windows EXE".
5. Click "Run workflow" (if it has not started automatically).
6. Wait for the green success check.
7. Open the completed workflow run and download the artifact named
   "BeneficiaryVerification-Windows-x64".
8. Extract the downloaded artifact ZIP. It contains:
   BeneficiaryVerification.exe

RUN:
Double-click BeneficiaryVerification.exe on a Windows 10/11 64-bit computer.
No Python installation is needed on that target computer.

NOTE:
The EXE may be flagged by Windows SmartScreen because it is an unsigned
custom-built application. Only run it if you trust the source and build.
