# Step-by-Step Manual for Installing VS Code and Python

## Step 1: Install Python

### Download Python:
- Go to the official Python website: [https://www.python.org/downloads/](https://www.python.org/downloads/).
- The website should automatically suggest the latest version for your operating system (Windows, macOS, or Linux). Click the **"Download Python [version number]"** button.

### Run the Installer:
- Once the installer is downloaded, locate the file and open it.
- **Important:** On the first screen of the installer, check the box that says **"Add Python to PATH"**. This step is crucial for ensuring that Python works correctly with VS Code.

### Install Python:
- Click on **"Install Now"** to start the installation process.
- Wait for the installation to complete. This may take a few minutes.
- After the installation is complete, you can click **"Close"**.

### Verify Python Installation:
- Open a terminal or command prompt:
  - **Windows:** Press `Windows + R`, type `cmd`, and hit Enter.
  - **macOS/Linux:** Open the Terminal application.
- Type the following command and press Enter:
    ```bash
    python --version
    ```
- You should see the installed Python version number (e.g., Python 3.11.x). This confirms that Python is installed and correctly added to your system's PATH.

## Step 2: Install Visual Studio Code (VS Code)

### Download VS Code:
- Go to the official VS Code website: [https://code.visualstudio.com/](https://code.visualstudio.com/).
- Click the **"Download for [Your OS]"** button. The website should automatically detect your operating system (Windows, macOS, or Linux).

### Run the Installer:
- Once the VS Code installer is downloaded, locate the file and open it.
- Follow the installation prompts:
  - **Windows:**
    - Accept the license agreement.
    - Choose the installation location (or use the default).
    - **Important:** Check the box that says **"Add to PATH"** and any other options like "Create a desktop icon" if desired.
    - Click **"Install"**.
  - **macOS/Linux:** Drag the VS Code icon to the Applications folder or follow the on-screen instructions.

### Launch VS Code:
- Once the installation is complete, launch VS Code:
  - **Windows:** You can open it from the Start menu or desktop shortcut.
  - **macOS:** Open it from the Applications folder or search for it using Spotlight.
  - **Linux:** Launch it from your applications menu or by typing `code` in the terminal.

## Step 3: Setting Up Python in VS Code

### Install Python Extension in VS Code:
- When you first open VS Code, you may be prompted to install recommended extensions. If the Python extension is suggested, click **"Install"**.
- If not, you can manually install it:
  - Click on the **Extensions** view icon on the sidebar (or press `Ctrl+Shift+X` / `Cmd+Shift+X`).
  - In the search box, type "Python" and look for the extension by Microsoft.
  - Click **"Install"**.

### Verify Python Extension Installation:
- Open a new file by clicking **File > New File**.
- Save the file with a `.py` extension (e.g., `test.py`).
- VS Code should automatically detect Python and display a prompt to select a Python interpreter. If it doesn't, click on the Python version displayed in the bottom-left corner and select the installed Python interpreter.

### Run a Python Script in VS Code:
- Type the following code in your `test.py` file:
    ```python
    print("Hello, World!")
    ```
- Right-click in the editor and select **"Run Python File in Terminal"**.
- The output `"Hello, World!"` should appear in the terminal at the bottom of the VS Code window. This confirms that everything is set up correctly.

## Step 4: Setting Up Jupyter Notebooks (Optional, Recommended)

### Install Jupyter Extension:
- Open the Extensions view again (`Ctrl+Shift+X` / `Cmd+Shift+X`).
- Search for "Jupyter" and install the Jupyter extension by Microsoft.

### Creating and Running a Jupyter Notebook:
- In VS Code, go to **File > New File** and save the file with a `.ipynb` extension (e.g., `notebook.ipynb`).
- This will create a new Jupyter Notebook. You can now write and execute Python code in separate cells.

## Step 5: Explore and Customize VS Code (Optional)

### Install Additional Extensions:
- Depending on your needs, you can explore and install other extensions, such as GitHub integration, Markdown support, or specific language tools.

### Customize Settings:
- Explore the settings to customize your VS Code environment (e.g., themes, font size, key bindings).

## Final Step: Practice and Explore

- Explore VS Code by creating simple Python scripts and experimenting with basic Python operations.
- You can also use ChatGPT or other resources to help with any questions as they start coding.
