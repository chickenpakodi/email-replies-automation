# Email Automation with GPT, AI, and Python

**Project Overview**  
Developed an email automation script using Python that leverages the OpenAI GPT model to generate intelligent replies to incoming emails. This solution enhances email management by automating responses, thereby saving time and improving communication efficiency. The script utilizes the SMTP and IMAP protocols for sending and receiving emails, ensuring secure and reliable operation.

### Features
- **Automated Email Replies**: Automatically responds to unread emails with generated replies using OpenAI's GPT model.
- **IMAP and SMTP Integration**: Connects to email accounts securely for sending and receiving messages.
- **Customizable AI Responses**: Allows configuration of the AI's role and behavior, tailoring responses to specific user needs.
- **Email Body Extraction**: Efficiently extracts plain text from both multipart and regular emails for processing.

### Tech Stack
- **Python**: Programming language used for scripting the automation.
- **OpenAI API**: Provides access to GPT models for generating email responses.
- **IMAP**: Used for reading and managing emails in the inbox.
- **SMTP**: Used for sending emails.
- **email**: A built-in library in Python for managing email messages.
- **ssl**: Provides a secure context for sending emails.

### Project Structure
Below is a breakdown of the key components of the project:

1. **`mail_bot` Class**:
   - The main class containing methods for reading emails, generating replies using GPT, and sending emails. It encapsulates all functionalities required for the email automation process.

2. **`__init__` Method**:
   - Initializes the email bot with necessary configurations, including API keys, email server details, and folder names for sent and inbox emails.

3. **`reply_to_emails` Method**:
   - Connects to the email server, retrieves unread emails, generates replies using the `ai_responder` method, and sends responses back to the original senders.

4. **`get_email_body` Method**:
   - Extracts the plain text body from email messages, accommodating both multipart and simple emails.

5. **`send_email` Method**:
   - Constructs the email message and sends it to the specified recipient. It also logs the sent email in the designated sent folder.

6. **`ai_responder` Method**:
   - Interacts with the OpenAI API to generate replies based on the content of the incoming email. It configures the AI's behavior and processes the response.

7. **`if __name__ == "__main__"` Block**:
   - Sets up the necessary variables and creates an instance of the `mail_bot` class, executing the email reply process.

### Conclusion
This Email Automation project demonstrates a powerful application of AI in streamlining email communications. By integrating the OpenAI GPT model, the bot efficiently manages email responses, making it a valuable tool for personal or business use. The project exemplifies best practices in Python scripting, API integration, and secure email handling.

### Installation
The program is ready to use. You only need to:
1. Install the OpenAI library:
   ```bash
   pip install openai
