# Build Script Instructions

This script automates the process of converting a Python script into a standalone executable using PyInstaller.

## Prerequisites

1. **Python**: Ensure Python is installed and added to your system's PATH.  
   Check installation:
   ```bash
   python --version
   ```
2. **PyInstaller**: Install PyInstaller if not already installed:
   ```bash
   pip install pyinstaller
   ```

## How to Use

1. Save this build script (e.g., `PY2EXE.py`) in the same directory as your Python script.
2. Open the Command Prompt (cmd).
3. Navigate to the directory containing the script:
   ```bash
   cd path\to\your\scripts
   ```
4. Run the script:
   ```bash
   python build_script.py
   ```
5. When prompted, enter the name of the Python script you want to build into an executable (e.g., `example.py`).

### Example Execution
```bash
C:\path\to\scripts> python PY2EXE.py
Enter the name of the python script to build into an exe: example.py
Executable can be found under example/dist/example.exe
```

## Output

- The executable will be located in the `dist` folder of the script's directory.
- For example, if your Python script is named `example.py`, the generated executable will be:
  ```
  example/dist/example.exe
  ```

## Notes

- Ensure that all dependencies used in your Python script are installed in your Python environment.
- The script uses PyInstaller's `--onefile` option, which packages all dependencies into a single executable file.
