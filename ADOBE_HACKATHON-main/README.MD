# AI-Powered SQL Query Generator and Corrector

This project is a Streamlit-based web application that uses the Groq API and a PostgreSQL database to generate and correct SQL queries based on natural language input. It is designed to help users interact with databases using natural language and automatically correct SQL queries.

---

## Features

1. **Natural Language to SQL**:
   - Translates natural language queries into SQL queries using the Groq API.
   - Supports complex queries involving multiple tables and conditions.

2. **SQL Query Correction**:
   - Corrects incorrect SQL queries based on the database schema and examples.

3. **Database Integration**:
   - Connects to a PostgreSQL database to fetch schema information and validate queries.

4. **Streamlit UI**:
   - Provides an intuitive user interface for inputting natural language queries and viewing generated or corrected SQL queries.

---

## Prerequisites

Before running the project, ensure you have the following installed:

1. **Python 3.8+**
2. **PostgreSQL** (for database connection)
3. **Required Python Libraries**:
   - Install the required libraries using the following command:
     ```bash
     pip install streamlit pandas psycopg2 groq
     ```

4. **Groq API Key**:
   - Obtain a Groq API key from [Groq Cloud](https://groq.com/).
   - Replace the placeholder `groq_api_key` in the code with your actual API key.

5. **PostgreSQL Database**:
   - Set up a PostgreSQL database and update the connection details in the `connect_to_db` function:
     ```python
     conn = psycopg2.connect(
         dbname="your_db_name",
         user="your_db_user",
         password="your_db_password",
         host="localhost",
         port="5432"
     )
     

# ADOBE_HACKATHON
