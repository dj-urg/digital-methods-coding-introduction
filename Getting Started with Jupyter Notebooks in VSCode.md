
# Getting Started with Jupyter Notebooks in VSCode

This guide will help you get started with creating and running a Jupyter notebook in Visual Studio Code (VSCode), assuming you’ve just installed Python and opened VSCode for the first time. We’ll walk through the entire process, from installing the necessary extensions to actually running code cells within a notebook.

## Prerequisites

- **Python Installed:**  
  Make sure that Python is already installed on your machine. You can verify this by opening your terminal (on Windows, Command Prompt or PowerShell; on macOS/Linux, your system terminal) and running:
  ```bash
  python --version
  ```
  If it shows a version number (e.g., `Python 3.10.0`), you have Python installed.

- **VSCode Installed:**  
  You should have Visual Studio Code installed and open on your machine. If not, you can download it from [https://code.visualstudio.com/](https://code.visualstudio.com/).

## Installing the Python and Jupyter Extensions

1. **Open the Extensions Panel in VSCode:**
   - On the left-hand side of VSCode, click the `Extensions` icon (it looks like four squares arranged in a grid).

2. **Search for the Python Extension:**
   - In the search bar at the top of the Extensions panel, type: `Python`.
   - Look for the official **Python** extension by Microsoft.
   - Click on the `Install` button.

3. **Search for the Jupyter Extension:**
   - Still in the Extensions panel, type: `Jupyter`.
   - Find the **Jupyter** extension by Microsoft.
   - Click `Install` to add it to VSCode.

The Python extension provides Python language support, and the Jupyter extension adds notebook functionality directly in VSCode.

## Creating a New Jupyter Notebook

1. **Command Palette:**
   - Open the Command Palette in VSCode by using `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (macOS).
   - Type: `Jupyter: Create New Blank Notebook` and select that option.
   
2. **Save Your Notebook:**
   - Once the blank notebook opens, save it by going to **File > Save As...**
   - Give it a name, for example `my_first_notebook.ipynb`, and choose a folder where you want to store it.

3. **Select a Python Kernel:**
   - At the top right corner of the notebook, you’ll see a button that says `Select Kernel`. Click it.
   - From the list of Python environments that appears, select the one where you installed Python (for most new installations, it will just be a default Python environment).
   - This will ensure that code runs against the chosen Python installation.

## Opening and Running an Existing Jupyter Notebook from a Repository

If the repository you cloned (or downloaded) contains a Jupyter notebook file (with the `.ipynb` extension), here’s what you do:

1. **Open the Folder in VSCode:**
   - In VSCode, go to **File > Open Folder...**.
   - Navigate to the folder where you cloned or saved the repository.
   - Click **Open** to load the entire project in VSCode.

2. **Locate the Notebook File:**
   - In VSCode’s left sidebar (the Explorer view), find the `.ipynb` file you want to open.
   - Click on it to open it in the editor panel.

3. **Select a Kernel:**
   - Once the notebook opens, ensure a Python kernel is selected as above.
   - If prompted, choose your installed Python environment.

## Running Code Cells

Inside a Jupyter notebook, code is organized into **cells**.

1. **Write Some Code:**
   - Click inside a cell and type a simple Python command, for example:
     ```python
     print("Hello, world!")
     ```

2. **Run the Cell:**
   - Hover your mouse over the left side of the cell. You’ll see a `Run Cell` button (a triangle “play” icon).
   - Click the `Run Cell` button.
   - Alternatively, you can use the keyboard shortcut:
     - **Ctrl+Enter** (Windows/Linux)
     - **Cmd+Enter** (macOS)

3. **View Outputs:**
   - Once you run the cell, its output (e.g., `Hello, world!`) will appear right below the cell.

## Tips and Tricks

- **Kernel/Interpreter Changes:**
  If you need to switch which Python environment you’re using, click on the kernel selector at the top right of the notebook and choose a different environment.

- **Installing Packages:**
  If your notebook requires additional packages, you can install them from within the VSCode terminal. For example:
  ```bash
  pip install requests
  ```
  Then switch back to your notebook and run cells using that package.

- **Saving Your Work:**
  Remember to regularly save your notebook with **File > Save** (or `Ctrl+S`/`Cmd+S`).

## Summary

- **Install Python, VSCode, and the Python & Jupyter extensions.**
- **Create or open a `.ipynb` file in VSCode.**
- **Select a Python kernel and run code cells directly within VSCode.**

With these steps, you’re ready to start exploring and running Jupyter notebooks right from within VSCode!
