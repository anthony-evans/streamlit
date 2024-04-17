# Example Streamlit app

## Prerequisites
1. **Python**: To run the Streamlit app, you need Python version 3.8 to 3.12.
2. **Install Python**: If Python is not already installed on your system, you can download and install it from the official Python website: [Python Downloads](https://www.python.org/downloads/). 

## Getting Started
1. **Open Terminal**: For Windows users, Right-click on the Command Prompt or Windows PowerShell icon and select "Run as administrator".
2. **Clone Project Repository**: Use following command to clone Project Repository:
   ```
   git clone <repository_url>
   ```

4. **Navigate to the Project Repository**: Use following command to navigate to the Project Repository:
   ```
   cd Streamlit-App-Template
   ```

5. **Create a Virtual Environment**: Run the following command to create a virtual environment named `venv`:
    ```bash
    # For Windows (without WSL)
    python -m venv venv
    
    # For everything else
    python3 -m venv venv
    ```

6. **Activate the Virtual Environment**: To activate the virtual environment, use the following command:
    ```bash
    # For Windows (without WSL)
    venv\Scripts\activate
    
    # For everything else
    source venv/bin/activate
    ```
   After running this command, `(venv)` should appear at the beginning of your command prompt, indicating that the virtual environment is active.

7. **Install Dependencies**: Once the virtual environment is activated, install the required dependencies using the following command:
    ```bash
    pip install -r requirements.txt
    ```
   This will install all the necessary Python packages specified in the `requirements.txt` file.

## Running the Streamlit App
1. **Start the Streamlit App**: To run the Streamlit app, use the following command:
    ```bash
    streamlit run app.py
    ```
   This command will start the Streamlit server and open your default web browser to display the app. If the app does not open automatically in your browser, you can manually open it by copying the local URL provided in the terminal and pasting it into your browser's address bar.
   
## Adding Requirements
1. **Add New Requirements**: To add new requirements, update the `requirements.in` file and regenerate the `requirements.txt` lock file with:
    ```bash
    pip-compile
    ```
2. Then update the virtual environment with:
    ```bash
    pip install -r requirements.txt
    ```
