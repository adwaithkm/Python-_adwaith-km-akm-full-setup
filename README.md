Python Project Setup Guide

Author: AKM (adwaith km )

This guide provides comprehensive steps for setting up a Python project, including Python installation, environment configuration, library installations, and troubleshooting tips.


---

1. Install Python

1. Download the latest version of Python from python.org.


2. During the installation, check the box to "Add Python to PATH".




---

2. Verify Python Installation

To ensure Python is installed correctly, run:

python --version

or

python3 --version


---

3. Upgrade Pip and Install Essential Tools

Run these commands to ensure your tools are up-to-date:

python -m pip install --upgrade pip setuptools wheel  
python -m pip install setuptools-rust


---

4. Create a Virtual Environment

Using a virtual environment isolates your project dependencies.

Steps:

1. Navigate to your project folder:

cd path/to/your/project


2. Create a virtual environment:

python -m venv .venv


3. Activate the virtual environment:

Windows:

.venv\Scripts\activate

macOS/Linux:

source .venv/bin/activate



4. Confirm activation:
You should see (.venv) at the beginning of your terminal prompt.




---

5. Install Project Dependencies

Ensure all required libraries are installed:

1. If a requirements.txt file is available:

pip install -r requirements.txt


2. Install specific libraries manually (e.g., OpenCV):

pip install opencv-python




---

6. Run Your Python Application

To execute your project:

python your_script_name.py


---

7. Adding Python to PATH (if not done during installation)

1. Open System Properties → Environment Variables.


2. Under System Variables, find Path and click Edit.


3. Add the following paths:

Python installation directory (e.g., C:\Python\)

Scripts directory (e.g., C:\Python\Scripts)





---

8. Common Troubleshooting

ModuleNotFoundError

If you encounter a ModuleNotFoundError, install the missing library:

pip install library_name

Environment Activation Issues

Ensure you are in the correct directory where the .venv folder is located.

Re-run the activation command.



---

9. Additional Commands

Upgrading a Specific Package

pip install --upgrade package_name

Listing Installed Packages

pip list

Deactivating the Virtual Environment

To exit the virtual environment:

deactivate


---

10. Feedback and Contribution

Feel free to contribute or provide feedback by opening an issue in the repository.


---

Maintained by: AKM


---
