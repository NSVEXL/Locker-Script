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
    #!/bin/bash

    # Initializing variables to store user input
    username=""
    companyname=""
    pin=""

    #    Starting a loop to gather information in 3 steps
    for i in {1..3}; do
    # Logic to prompt for different data based on the loop iteration
    if [ "$i" -eq 1 ]; then
        read -p "Enter your Username: " username
    elif [ "$i" -eq 2 ]; then
        read -p "Enter your Company name: " companyname
    else
        # Using -s flag is recommended for PINs, but keeping it simple for the exercise
        read -p "Enter your PIN: " pin
    fi
    done

    # Validating the credentials against hardcoded values
    if [ "$username" = "Neo" ] && [ "$companyname" = "Matrix" ] && [ "$pin" = "0123" ]; then
    echo "---------------------------------------"
    echo "Authentication Successful."
    echo "Access granted. Welcome back, Neo."
    echo "---------------------------------------"
    else
    echo "---------------------------------------"
    echo "Authentication Denied!!"
    echo "Invalid credentials. Access rejected."
    echo "---------------------------------------"
    exit 1
    fi
    ```

2.  **Grant execution permissions:**
    ```bash
    chmod +x locker_script.sh
    ```

3.  **Run the script:**
    ```bash
    ./locker_script.sh
    ```

## 📝 Disclaimer

This script was created for educational purposes. Note that hardcoding credentials (like the PIN in this script) is not a secure practice for real-world production environments and is used here strictly to demonstrate logic flow.

---
*Learning and building in public. 🚀*
