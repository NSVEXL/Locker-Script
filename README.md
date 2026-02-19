# Simple Bash Authentication Logic

This project is a practical exercise completed as part of my learning journey on **TryHackMe**. It demonstrates fundamental scripting concepts in Bash, focusing on user input handling and control flow.

## 🛠️ Description

The script simulates a basic authentication gateway. It prompts the user for three specific pieces of information (Username, Company Name, and PIN) using a loop and validates them against predefined credentials.

## 🧠 Key Concepts Applied

* **Variable Initialization:** Setting up placeholders for user data.
* **For Loops:** Iterating through a set range to trigger different input prompts.
* **Conditional Logic (`if/elif/else`):** Directing the script's behavior based on the current iteration and validating final credentials.
* **Logical Operators:** Using `&&` (AND) to ensure all security conditions are met simultaneously.

## 🚀 How to Use

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd YOUR_REPO_NAME
    ```

2.  **Grant execution permissions:**
    ```bash
    chmod +x authentication.sh
    ```

3.  **Run the script:**
    ```bash
    ./authentication.sh
    ```

## 📝 Disclaimer

This script was created for educational purposes. Note that hardcoding credentials (like the PIN in this script) is not a secure practice for real-world production environments and is used here strictly to demonstrate logic flow.

---
*Learning and building in public. 🚀*
