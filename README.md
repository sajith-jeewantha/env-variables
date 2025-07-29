# 🔐 Secure Configuration with Environment Variables

This project follows industry best practices for managing sensitive data such as API keys, database credentials, and secret tokens.

---

## ✅ Why Use Environment Variables?

Hardcoding secrets directly in source code is insecure and error-prone. Instead, this project uses environment variables to:

- ❌ Avoid hardcoding secrets in code
- ✅ Securely manage environment-specific configuration
- ✅ Prevent accidental exposure of sensitive data
- ✅ Improve portability across development, staging, and production environments

---

## 📁 Where to Add Environment Variables

Environment-specific values are stored in a `.env` file located inside the `resources/` directory.

- **`resources/.env`**:  
  Contains actual environment values. This file is **not committed** to version control. It must be created locally by each developer or set securely in the deployment environment.

- **`resources/.env.example`**:  
  A safe, shareable template file that defines all required variables (without real values). This file **is committed** to the repository to help developers set up their local environment quickly and consistently.

---

## 🚀 Getting Started

1. **Copy the example file to create your own local environment file:**

   ```bash
   cp resources/.env.example resources/.env
