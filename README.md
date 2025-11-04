# IBM-EDU - Data Science Tools and Ecosystem

This repository contains IBM Data Science educational materials, including Jupyter notebooks and course resources.

## How to Connect to VSCode

This guide will help you set up and connect this repository to Visual Studio Code (VSCode) for working with Jupyter notebooks and other materials.

### Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/) installed on your computer
- [Git](https://git-scm.com/) installed on your computer
- [Python](https://www.python.org/downloads/) (version 3.7 or higher recommended)

### Step 1: Clone the Repository

1. Open VSCode
2. Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac) to open the Command Palette
3. Type "Git: Clone" and select it
4. Enter the repository URL: `https://github.com/UJ101/IBM-EDU.git`
5. Choose a local folder where you want to save the repository
6. Click "Open" when prompted to open the cloned repository

**Alternative - Using Terminal:**
```bash
git clone https://github.com/UJ101/IBM-EDU.git
cd IBM-EDU
code .
```

### Step 2: Install Required VSCode Extensions

For the best experience working with Jupyter notebooks and Python files, install these extensions:

1. **Python** (by Microsoft)
   - Press `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac) to open Extensions
   - Search for "Python" and install the official Microsoft extension

2. **Jupyter** (by Microsoft)
   - Search for "Jupyter" and install the official Microsoft extension
   - This enables you to open and run `.ipynb` files directly in VSCode

3. **Jupyter Notebook Renderers** (by Microsoft) - Optional
   - Provides rich output rendering for notebooks

### Step 3: Set Up Python Environment

1. Open the integrated terminal in VSCode: Press `Ctrl+\`` (Control and backtick key) or use menu `Terminal > New Terminal`
2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   ```
3. Activate the virtual environment:
   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - Mac/Linux:
     ```bash
     source venv/bin/activate
     ```
4. Install Jupyter and required packages:
   ```bash
   pip install jupyter notebook ipykernel
   ```

### Step 4: Open and Run Jupyter Notebooks

1. In the VSCode Explorer (`Ctrl+Shift+E`), navigate to the notebook file (e.g., `Jupyter_Notebook (1).ipynb`)
2. Click on the notebook file to open it
3. VSCode will automatically detect it as a Jupyter notebook
4. Select a Python kernel:
   - Click on "Select Kernel" in the top right corner
   - Choose your Python environment (the virtual environment you created)
5. Run cells by clicking the "Run" button next to each cell or press `Shift+Enter`

### Step 5: Working with the Repository

- **View Files**: Use the Explorer panel on the left (`Ctrl+Shift+E`)
- **Search**: Use `Ctrl+Shift+F` to search across all files
- **Source Control**: Use the Source Control panel (`Ctrl+Shift+G`) to commit and push changes
- **Terminal**: Use the integrated terminal (press `Ctrl+\`` or Control and backtick key) for command-line operations

### Recommended VSCode Settings for Jupyter

Add these to your VSCode settings (File > Preferences > Settings or `Ctrl+,`):

```json
{
    "jupyter.askForKernelRestart": false,
    "notebook.cellToolbarLocation": {
        "default": "right",
        "jupyter-notebook": "left"
    },
    "files.autoSave": "afterDelay"
}
```

### Troubleshooting

**Problem: Jupyter notebook won't open or run**
- Solution: Ensure the Python and Jupyter extensions are installed
- Solution: Install Jupyter: `pip install jupyter notebook`
- Solution: Restart VSCode after installing extensions

**Problem: Kernel not found**
- Solution: Make sure Python is installed and added to PATH
- Solution: Select the correct Python interpreter: `Ctrl+Shift+P` > "Python: Select Interpreter"
- Solution: Install ipykernel: `pip install ipykernel`

**Problem: Git clone fails**
- Solution: Ensure Git is installed and configured
- Solution: Check your internet connection
- Solution: Use HTTPS URL instead of SSH if you don't have SSH keys set up

**Problem: Can't see notebook output or images**
- Solution: Install "Jupyter Notebook Renderers" extension
- Solution: Restart the kernel and run all cells again

### Additional Resources

- [VSCode Jupyter Documentation](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
- [VSCode Python Tutorial](https://code.visualstudio.com/docs/python/python-tutorial)
- [Git in VSCode](https://code.visualstudio.com/docs/sourcecontrol/overview)

### Repository Contents

- `Jupyter_Notebook (1).ipynb` - Main Jupyter notebook for IBM Data Science course
- `IBM-CLASS FOLDER/` - Course screenshots showing completed notebook exercises (PNG images)

## Getting Started with the Notebooks

Once you have VSCode connected and set up:

1. Open `Jupyter_Notebook (1).ipynb`
2. Follow the instructions in the notebook
3. Complete the exercises as outlined in the IBM Data Science course
4. Save your work regularly

## Contributing

If you make improvements or corrections:

1. Create a new branch: `git checkout -b feature/your-feature-name`
2. Make your changes
3. Commit: `git commit -m "Description of changes"`
4. Push: `git push origin feature/your-feature-name`
5. Create a Pull Request

## License

This repository contains educational materials from IBM Data Science courses.
