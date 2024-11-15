
# Little Lemon App Development Guide

## Step-by-Step Instructions

### 1. **Set Up the Environment**
   - **Windows:**
     ```bash
     python -m venv env
     ```
   - **MacOS:**
     ```bash
     python3 -m venv env
     ```

### 2. **Activate the Environment**
   - **Windows:**
     ```bash
     .\env\Scripts\activate
     ```
   - **MacOS:**
     ```bash
     source env/bin/activate
     ```

### 3. **Install Django**
   - **Windows:**
     ```bash
     pip install django
     ```
   - **MacOS:**
     ```bash
     pip3 install django
     ```

   - **Confirm Installation:**
     - **Windows:**
       ```bash
       python -m django version
       ```
     - **MacOS:**
       ```bash
       python3 -m django version
       ```

### 4. **Create a Django Project**
   ```bash
   django-admin startproject <project_name> .
   ```

### 5. **Add a Django App**
   - **Option 1 (Preferred):**
     ```bash
     python manage.py startapp <app_name>
     ```
   - **Option 2:**
     - **Windows:**
       ```bash
       python -m django startapp <app_name>
       ```
     - **MacOS:**
       ```bash
       python3 -m django startapp <app_name>
       ```

### 6. **Run the Development Server**
   - Navigate to the project directory:
     ```bash
     cd <project_name>
     ```
   - Start the server:
     - **Windows:**
       ```bash
       python manage.py runserver
       ```
     - **MacOS:**
       ```bash
       python3 manage.py runserver
       ```

### 7. **Deactivate the Environment**
   ```bash
   deactivate
   ```

---

## Overview of Project Goals

This guide is designed to help you create a fully functional Django-based website that showcases menu pages for the fictional "Little Lemon" restaurant. 

Key features include:
- A homepage linking to "About," "Menu," and "Book" pages via a navigation menu.
- A menu page displaying a list of items stored in the database, complete with their **Name**, **Price**, **Description**, and **Image**.
- A dedicated page for each menu item, accessible via clickable links on the menu page.
- Menu items displayed in alphabetical order.
- A footer section included on all pages.

---

## Submission and Peer Review Process

### Preparing Your Submission

1. **Export the Project:**
   - Use the "Lab Files" feature in the Coursera environment to select and download all your project files as a `.zip`.

2. **Locate the Project Folder:**
   - After extracting the downloaded `.zip`, find the `littlelemon` folder at:
     ```
     Files > Files > home > coder > project
     ```

3. **Compress the Folder:**
   - Zip the `littlelemon` folder to prepare it for submission.

4. **Submit on Coursera:**
   - Go to the assignment page and upload your zipped project file under the **My Submission** tab.

---

### Reviewing Peer Projects

1. **Access Assigned Projects:**
   - In the "Review assignments" section, download the `.zip` files of two peer submissions.

2. **Set Up in Sandbox Lab:**
   - Use the Peer Review Sandbox to upload and run the Django projects.

3. **Test and Evaluate:**
   - Open the development server at `http://127.0.0.1:8000/` and verify the following:
     - Does the homepage link to the menu page?
     - Are menu items displayed alphabetically with names, prices, and clickable links?
     - Do individual menu item pages show all relevant details?
     - Is there a footer section on every page?

---

### Providing Constructive Feedback

Effective feedback should focus on functionality and offer actionable suggestions for improvement. For example:

- *"The project met most of the requirements, but on the menu page, the items were not displayed as clickable links. You might consider using Django's `href` attribute in the template to fix this issue."*

---

## Example Output

### Menu Page (`http://127.0.0.1:8000/menu/`)
The menu page should display all items stored in the database, sorted alphabetically and accompanied by their prices and links to individual item pages.

![Menu Page Example](https://prod-files-secure.s3.us-west-2.amazonaws.com/de1096b7-5a86-4b89-9025-3b4d9abb6eec/dTpn_YnHSrGRTqAIFhr3fQ_4515bd5fa705424e93df69023f33fce1_peer-review-menu-page.png)

### Menu Item Page (`http://127.0.0.1:8000/menu_item/1/`)
Each menu item page should display its name, price, description, and image.

![Menu Item Page Example](https://prod-files-secure.s3.us-west-2.amazonaws.com/de1096b7-5a86-4b89-9025-3b4d9abb6eec/4579cd26-8aa6-4825-91b6-719a5b29849f/ix6y6CCNRTaszL_eBNW7eA_8b1855e7e98a46ec9b8f5f4a9e04f2e1_peer-review-menu-item-page.png)

---

This guide ensures clarity and improved readability while emphasizing the essential steps and evaluation criteria for creating and reviewing a Django project.
