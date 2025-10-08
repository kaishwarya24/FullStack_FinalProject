# SAGA- Your AI Story Co-Author

SAGA is an interactive storytelling web application that allows users to co-create stories with AI. Users can provide the beginning of a story, select a personality for the AI co-author, and let the AI continue the story. Stories can be saved, viewed in a personal dashboard, and downloaded as text files.  

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/48a433a1-ead1-4010-bd57-6bdb0b970ee0" alt="Image 1" width="800"/></td>
    <td><img src="https://github.com/user-attachments/assets/6ba8f30a-6f00-438a-976c-f85cfa838b4b"  alt="Image 2" width="800"/></td></tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/3499aa42-5fee-45d7-90d9-2e47e2ddac27" alt="Image 3" width="800"/></td>
   <td><img src="https://github.com/user-attachments/assets/f93adff1-2b3e-45b1-9afe-7b002dded433" alt="Image 4" width="800"/></td>
  </tr>
    <tr>
    <td><img src="https://github.com/user-attachments/assets/3a717e77-f7e6-497e-9b56-8e79681d162f" alt="Image 5" width="800"/></td>
    <td><img src="https://github.com/user-attachments/assets/1d53862f-3299-475d-96ea-3f4c28a52770" alt="Image 6" width="800"/></td>
  </tr>
</table>

---

## Core Features
| Feature | Description |
|---------|------------|
|  **Story Input** | Users type the start of the story. |
|  **AI Continuation** | The AI extends the story using OpenAI or fallback mock responses. |
| **Personality Selector** | Users choose the AI co-author style: Sarcastic, Romantic, Horror, Whimsical, and more. |
|  **Regenerate Button** | Generates a new continuation without losing user input. |
|  **Save to Dashboard** | Stores full story along with AI personality in SQLite database. |
|  **Dashboard View** | Displays saved stories, with options to view, delete, or download. |
|  **User Authentication** | Register, login, and logout securely using Flask-Login and hashed passwords. |

---

## Technologies Used

- **Backend:** Python, Flask  
- **Database:** SQLite (via SQLAlchemy)  
- **Authentication:** Flask-Login, Werkzeug Security  
- **AI Integration:** OpenAI API (GPT-3.5-turbo) with fallback mock responses  
- **Frontend:** HTML, CSS, Bootstrap  
- **Environment Management:** python-dotenv  

---

## AI Personalities

Some of the available AI personalities for storytelling:

- Shakespeare  
- Hemingway  
- Tolkien  
- Comedy  
- Thriller  
- Sci-Fi  
- Rajkumar Hirani  
- S.S. Rajamouli  
- Zoya Akhtar  
- Anurag Kashyap  
- Karan Johar  

Each personality influences the style, tone, and narrative approach of the AI continuation.

---

## Setup Instructions

1. **Clone the repository**  
```bash
git clone https://github.com/kaishwarya24/SAGA-AI.git
cd SAGA
```
2. **Create a virtual environment**
   ```bash
   python -m venv venv
    venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

   
4. **Set up environment variables**
   ```bash
   OPENAI_API_KEY=your_openai_api_key_here
   SECRET_KEY=your_flask_secret_key_here

   ```
5. **Initialize the database**
   ```bash
   python
    >>> from app import db
    >>> db.create_all()
    >>> exit()

   ```
6. **Run the Flask application**
```bash
  python app.py
```
7. **Access the application**
    ```bash
    http://127.0.0.1:5000/

    ```
