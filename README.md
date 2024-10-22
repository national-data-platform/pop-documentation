# Generating and Running the POP Setup Script

This guide will walk you through generating a setup script for your Point of Presence (POP) and running it on your server. Follow these simple steps to get everything up and running smoothly.

## Step 1: Access the National Data Platform

![Step 1](./1.jpeg)
1. Open your web browser and navigate to [nationaldataplatform.org](https://nationaldataplatform.org).

## Step 2: Login

![Step 2](./2.jpeg)
2. Click on the **Log in/Register** button to sign in with your credentials.

## Step 3: Navigate to POPs

![Step 3](./3.jpeg)
3. Once logged in, locate and click on **POPs** in the sidebar or main navigation.

## Step 4: Choose POP Setup

![Step 4](./4.jpeg)
4. You will see an option to choose between POP (Point of Presence) or sciDX (Scientific Data Exchange). Select **POP** to proceed.

## Step 5: Fill in the Required Fields

![Step 5](./5.jpeg)
5. A form will appear asking for specific details:
   - **Catalog Username**: Enter your catalog username.
   - **Catalog Password**: Enter your catalog password.
   - **IDP Client ID**: Enter the client ID for the Identity Provider.
   - **IDP Client Secret**: Enter the client secret.
   - **Realm Name**: Enter the appropriate realm name.

## Step 6: Generate the Script

![Step 6](./6.jpeg)
6. Fill in the required fields and then click on the **Generate Script** button.
7. After a few moments, the setup script will be generated. Copy the script from the screen.

## Step 7: Log in to Your Server

![Step 7](./7.jpeg)
8. Log in to your server where you want to deploy the POP setup. You will need to have **sudo** permissions.

## Step 8: Save the Script
9. On your server, open a text editor (like `nano` or `vim`) and paste the copied script. Save the file as `setup.sh`.

## Step 9: Run the Setup Script

![Step 8](./8.jpeg)
10. Run the script by executing the following command:
   ```bash
   sudo bash setup.sh
   ```
   
This will initiate the setup process of your POP environment.

## Requirements for Running the Script
- You need **sudo** privileges. If you are not a sudo user, make sure you have the following tools and permissions:
  - **Docker** (recent version)
  - **Docker Compose** (recent version)
  - **Uvicorn** (recent version)
  - **PIP** (recent version)
  - **Python 3** (recent version)
  - **Git** (recent version)
  - **Ports 8000 and 8443** should be open
  - **Write permissions** on the server

**Note**: The script is tested on **Ubuntu**. If you plan to run it on other systems, you may need to modify it accordingly to fit your operating system.

## Need Help?
If you encounter any issues, please refer to the documentation provided on the platform or contact support.

