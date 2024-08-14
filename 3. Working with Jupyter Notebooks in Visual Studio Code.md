# Working with Jupyter Notebooks in Visual Studio Code

## Introduction to Jupyter Notebooks

### What is a Jupyter Notebook?

A Jupyter Notebook is an open-source, web-based application that allows you to create and share documents that contain live code, equations, visualizations, and narrative text. It's an incredibly powerful tool used for data cleaning and transformation, numerical simulation, statistical modeling, machine learning, and much more.

### Key Features of Jupyter Notebooks

- **Interactive Code Execution**: Write and execute code in a cell-by-cell manner, allowing you to see results immediately and experiment easily.
- **Rich Text Support**: Use Markdown to include formatted text, images, and even LaTeX equations directly alongside your code.
- **Visualization Integration**: Easily visualize data with libraries like Matplotlib, Seaborn, and Plotly, all within the notebook.
- **Easy Sharing**: Share your notebooks with others, including the code, outputs, and visualizations.

## Setting Up Jupyter Notebooks in Visual Studio Code

### Step 1: Install Python

Before you can work with Jupyter Notebooks in VS Code, you need to have Python installed on your system. If you haven't already installed Python, please refer to the [Step-by-Step Manual for Installing VS Code and Python](https://github.com/dj-urg/digital-methods-coding-introduction/blob/main/getting-started.md) for detailed instructions.

### Step 2: Install the Jupyter Extension

1. **Open Visual Studio Code**.
2. Click on the **Extensions** icon in the Activity Bar on the side of the window (or press `Ctrl+Shift+X` / `Cmd+Shift+X`).
3. In the search box, type "Jupyter".
4. Look for the extension named **Jupyter** by Microsoft.
5. Click **Install**.

The Jupyter extension integrates with the Python extension and allows you to create, open, and run Jupyter Notebooks directly in VS Code.

### Step 3: Creating a New Jupyter Notebook

1. **Open VS Code**.
2. Go to **File > New File**.
3. Save the file with a `.ipynb` extension (e.g., `my_notebook.ipynb`). This tells VS Code to treat the file as a Jupyter Notebook.
4. Once saved, the notebook interface will open in VS Code.

### Step 4: Working with Jupyter Notebooks in VS Code

#### 4.1 Understanding the Interface

- **Code Cells**: These are the primary components where you write and execute code. Click on a cell and type your Python code. Press `Shift + Enter` to execute the code and move to the next cell.
- **Markdown Cells**: These allow you to add formatted text to your notebook. To create a Markdown cell, click on a cell, and change the cell type to "Markdown" using the dropdown menu at the top.
- **Output Cells**: After running a code cell, the output (whether it's text, a plot, or an error message) will appear directly below the code cell.

#### 4.2 Running Code

- To execute a single cell, click on the cell and press `Shift + Enter`.
- To run all cells sequentially, use **Run All Cells** from the command palette or the toolbar.
- To restart the kernel (the computational engine running your code), click on the kernel status in the top right corner and select "Restart Kernel". This is useful if you want to clear all variables and start fresh.

#### 4.3 Using Markdown for Documentation

Markdown cells can be used to add headers, lists, links, images, and more:

- **Headers**: Use `#` for headers (e.g., `# Header 1`, `## Header 2`).
- **Bold and Italics**: Use `**text**` for bold and `*text*` for italics.
- **Lists**: Use `-` for bullet points and `1.` for numbered lists.
- **Links**: `[Link Text](URL)`
- **Images**: `![Alt Text](image_url)`
- **LaTeX Equations**: Wrap your LaTeX code with `$$` for block equations or `$` for inline equations (e.g., `$$E = mc^2$$`).

#### 4.4 Visualizing Data

One of the powerful features of Jupyter Notebooks is the ability to visualize data inline. Here's how you can do it:

```python
import matplotlib.pyplot as plt
import pandas as pd

# Example data: Public trust in government over years
data = {
    "Year": [2000, 2005, 2010, 2015, 2020],
    "Trust_in_Government": [45, 40, 35, 30, 25]  # Percentage of people who trust the government
}

# Convert the data into a DataFrame
df = pd.DataFrame(data)

# Plotting the data
plt.plot(df["Year"], df["Trust_in_Government"], marker='o')

# Adding title and labels
plt.title("Public Trust in Government Over Time")
plt.xlabel("Year")
plt.ylabel("Percentage of People Who Trust the Government")
```

### Step 5: Example Exercise - Analyzing YouTube Video Categories

In this exercise, you will learn how to load a CSV file containing YouTube video data, categorize the types of videos, and visualize the distribution of video categories. This will give you hands-on experience with basic data manipulation and analysis in a Jupyter Notebook.

#### 5.1. Install Required Libraries

Before starting, make sure you have the necessary Python libraries installed. You can do this directly in your Jupyter Notebook by running the following command:

```python
!pip install pandas matplotlib
```

#### 5.2. Load the Dataset

For this exercise, you can use a simple CSV file with two columns: `video_title` and `video_category`. Here’s how you can load the CSV file into a Pandas DataFrame:

```python
import pandas as pd

# Load the dataset
df = pd.read_csv('youtube_videos.csv')

# Display the first few rows of the dataset
df.head()
```

#### 5.3. Count the Number of Videos in Each Category

Next, you’ll count the number of videos in each category. This step helps you understand the distribution of video types in the dataset.

```python
# Count the number of videos in each category
category_counts = df['video_category'].value_counts()

# Display the counts
category_counts
```

#### 5.4. Visualize the Video Category Distribution

You can now visualize the distribution of video categories by creating a bar chart.

```python
import matplotlib.pyplot as plt

# Plot the distribution of video categories
category_counts.plot(kind='bar', edgecolor='black')
plt.title('Distribution of YouTube Video Categories')
plt.xlabel('Video Category')
plt.ylabel('Number of Videos')
plt.show()
```

#### 5.5. Interpret the Results

Take a look at the bar chart you generated:

Questions to consider:
- Which video category is the most common?
- How diverse are the video categories in the dataset?
- What does this distribution tell you about the content being uploaded?

This simple exercise introduces you to loading data, performing basic categorical analysis, and visualizing results—all essential skills in content analysis and media studies.
