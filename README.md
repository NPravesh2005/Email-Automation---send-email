# Experiment: Email Automation - Send Mail using UiPath Studio

## Aim
To automate sending an email using UiPath Studio via SMTP or Outlook activities.

## Materials Required
- UiPath Studio
- Access to an email account (e.g., Gmail, Outlook)
- SMTP server details (if using SMTP)
- UiPath.Mail.Activities package (installed by default)

## Procedure

1. **Create a New Project**  
   Open UiPath Studio and create a new Process project named `EmailAutomation`.

2. **Open Main.xaml**  
   Open `Main.xaml` in the workflow designer.

3. **Add Send SMTP Mail Message Activity (Using SMTP)**
   - Drag and drop the **Send SMTP Mail Message** activity.
   - Configure the following properties:
     - **To**: recipient email address (e.g., `example@domain.com`)
     - **Subject**: Email subject text
     - **Body**: Email body text
     - **From**: your email address
     - **SMTP Server**: SMTP server address (e.g., `smtp.gmail.com` for Gmail)
     - **Port**: SMTP port number (e.g., 587 for Gmail)
     - **SecureConnection**: Choose `Auto` or `StartTls`
     - **UserName** and **Password**: your email login credentials (preferably use secure credentials handling)
   - Optionally, attach files using the **Attachments** property.

4. **Alternative: Use Send Outlook Mail Message Activity**
   - If Outlook is installed and configured, use **Send Outlook Mail Message** activity.
   - Set **To**, **Subject**, **Body**, and optionally **Attachments**.

5. **Run the Workflow**  
   Save and run the workflow to send the email automatically.


## Output:

![Workflow](https://github.com/user-attachments/assets/38da3f87-3570-4160-b5e9-1d12ef921769)

![output (3)](https://github.com/user-attachments/assets/cb9c1cc7-5a88-4833-84df-dc46a60dcb75)

![Output (4)](https://github.com/user-attachments/assets/84a9f485-436e-4aeb-8d30-d545cd8b4271)

## Result
An email is sent automatically through the configured email server or Outlook client, demonstrating UiPath’s capability to automate email sending.
