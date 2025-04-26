# EzyBot 

[![Made with Prisma](http://made-with.prisma.io/indigo.svg)](https://prisma.io)

![Python](https://img.shields.io/badge/Python-3.11-blue)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-green)
![Prisma](https://img.shields.io/badge/ORM-Prisma-orange)
![Made with ❤️ in Nepal](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20in%20Nepal-green)

**EzyBot** is an intelligent, agentic chatbot developed as part of the **Rent Nepal** web service — a platform where users can add their rooms for rent or find available rooms.

## ✨ Features

- **Intent Detection**  
  EzyBot intelligently identifies whether the user wants to have a conversation or is looking for rooms to rent.

- **Room Search**  
  When asked about available rooms, EzyBot queries the MongoDB database using **Prisma ORM** and provides accurate results.

- **Conversation Handling**  
  EzyBot can engage in friendly, context-aware conversations when users simply want to talk.

- **Security Measures**  
  All dangerous code or malicious inputs are automatically filtered by the agent itself, ensuring safe interactions.

## 🛠️ Tech Stack

- **Backend**: Python
- **Database**: MongoDB
- **ORM**: Prisma ORM
- **Language Model API**: Llama-3.3-70b

## 📂 Project Structure

```
EZYBOT
├── assets/
│   ├── getTools.py
│   ├── promptNmessages.py 
│   └── query2response.py 
├── client/
│   └── client.py
├── dynamic_prisma_tools/ #Different method for using prisma
├── prisma/ 
│   └── schema.prisma 
├── .env
├── .gitignore
├── ezybot.py 
├── README.md
└── requirements.txt
```

## ⚙️ Installation and Setup

Follow the steps below to get EzyBot up and running locally:

1. **Clone the repository**
   ```bash
   git clone https://github.com/Page-Vishal/ezybot.git
   cd ezybot
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the environment variables**  
   Create a `.env` file in the project root with the following:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   DATABASE_URL=your_mongodb_connection_url_here
   ```

4. **Generate Prisma client**
   ```bash
   prisma generate
   ```

5. **Run EzyBot**
   ```bash
   python ezybot.py
   ```

---

## 📢 Notes

- The server infrastructure will be added later.
- Make sure MongoDB is running and accessible before querying.
- Prisma is used for smooth ORM-based database operations with MongoDB.

