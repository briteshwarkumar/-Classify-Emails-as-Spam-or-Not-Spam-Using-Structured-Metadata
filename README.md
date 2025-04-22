
---

## 📊 CSV Format

Your input CSV should contain structured metadata with the following columns:

| sender_domain | num_links | email_length | subject_length | is_spam |
|---------------|-----------|--------------|----------------|---------|
| gmail.com     | 2         | 1200         | 45             | 0       |
| cheapmeds.com | 10        | 500          | 20             | 1       |
| yahoo.com     | 1         | 850          | 35             | 0       |

- `sender_domain`: Domain of the sender's email
- `num_links`: Number of hyperlinks in the email
- `email_length`: Total number of characters in the email body
- `subject_length`: Number of characters in the subject
- `is_spam`: Target label (1 = spam, 0 = not spam)

---

## ⚙️ Installation

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/email-spam-classifier.git
cd email-spam-classifier
