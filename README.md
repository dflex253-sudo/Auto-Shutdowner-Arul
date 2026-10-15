# AutoShutdowner — legacy build attempt

This workflow tries to build with Python 3.8.10 and PyInstaller 5.13.2 on a Windows 2019 runner, which may improve compatibility with older Windows versions.

## How to use
1. Replace the files in your existing GitHub repository with these files, including `.github/workflows/build-windows.yml`.
2. Commit the changes to `main`.
3. Go to Actions → Build Windows EXE (Windows 7 legacy attempt) → Run workflow.
4. Download the `AutoShutdowner-x86-legacy` artifact first if your PC is 32-bit, or `AutoShutdowner-x64-legacy` if it is 64-bit.

## Important compatibility note
Windows 7 is obsolete and is no longer supported by current Python and packaging tools. This build is only a compatibility attempt, not a guarantee. If it still fails, use a supported Windows version or build on a Windows 7-compatible environment with an older toolchain. Never download an isolated `python311.dll` from third-party DLL sites.
