📚 Virtual Comic Store - Admin Panel
====================================

This project is a web-based admin panel built using **Flask**, **Flask-Admin**, and **Flask-Login**, which allows administrators to manage users, comics, and reviews in a virtual comic store. It uses SQLAlchemy ORM with support for SQLite (or any SQL-based database via DATABASE\_URL environment variable).

🚀 Features
-----------

*   🔐 Secure admin login using Flask-Login
    
*   📊 Dashboard with:
    
    *   Total users, comics, and reviews
        
    *   Pie chart showing genre distribution of comics
        
    *   Line chart showing user signup trends
        
*   🗃️ Admin panel for managing:
    
    *   Users
        
    *   Comics
        
    *   Reviews
        
*   🌱 Easy to set up and extend
    
*   🧩 Modular structure with SQLAlchemy models and route separation
    

🏗️ Tech Stack
--------------

*   Python 3.x
    
*   Flask
    
*   Flask-Admin
    
*   Flask-Login
    
*   SQLAlchemy
    
*   SQLite (default) / PostgreSQL / MySQL (optional via environment)
    

🧬 Project Structure
--------------------

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   csharpCopyEditvirtual-comic-store/  │  ├── app.py                   # Main Flask app with admin setup  ├── models.py                # SQLAlchemy models (User, Comic, Review)  ├── routes.py                # App routes (e.g., login, register)  ├── templates/  │   └── admin_dashboard.html # Custom admin dashboard  ├── static/                  # Static files (CSS/JS/images)  ├── requirements.txt         # Dependencies  └── README.md                # You're reading this!   `

⚙️ Setup Instructions
---------------------

### 1\. Clone the repository

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditgit clone https://github.com/your-username/virtual-comic-store.git  cd virtual-comic-store   `

### 2\. Create a virtual environment

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditpython -m venv venv  source venv/bin/activate  # On Windows use: venv\Scripts\activate   `

### 3\. Install dependencies

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditpip install -r requirements.txt   `

### 4\. Configure environment variables

Create a .env file or export them manually:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   envCopyEditSESSION_SECRET=your_secret_key  DATABASE_URL=sqlite:///comic_app.db  # Optional: change to your DB URL   `

### 5\. Run the app

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditpython app.py   `

Visit: [http://localhost:5000](http://localhost:5000)

📘 Models Overview
------------------

### User

*   id
    
*   username
    
*   email
    
*   password (hashed)
    
*   created\_at
    

### Comic

*   id
    
*   title
    
*   author
    
*   genre
    
*   release\_date
    

### Review

*   id
    
*   user\_id (FK)
    
*   comic\_id (FK)
    
*   rating
    
*   comment
    
*   created\_at
    

📈 Dashboard Charts (in admin\_dashboard.html)
----------------------------------------------

*   **Genre Distribution** (Pie Chart)
    
*   **User Signup Trend** (Line Chart by month)
    

Ensure your HTML template uses a charting library like **Chart.js** to visualize the data (not shown in code snippet above).

✅ To Do / Ideas
---------------

*   Add login/logout UI
    
*   Add role-based access (admin vs user)
    
*   Add search/filter in admin views
    
*   Use PostgreSQL in production
    

📄 License
----------

This project is licensed under the MIT License. Feel free to use, modify, and share it.

🙋‍♀️ Contributions
-------------------

Contributions are welcome! Fork the repo, make changes, and open a PR.

Let me know if you'd like a requirements.txt, a sample models.py, or admin\_dashboard.html starter template too.

4o