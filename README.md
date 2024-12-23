<div align="center">
  <div>
  <img src="./images/BlogLogo.svg" />
  </div>
</div>

# Blog Application Server
The Blog App is a backend for a blogging platform where users can write, update, and delete their blogs. The system will have two roles: Admin and User. The Admin has special permissions to manage users and their blogs, while users can perform CRUD operations on their own blogs. The backend will include secure authentication, role-based access control, and a public API for viewing blogs with search, sort, and filter functionalities.
## 🔬 Used Technologies
<div style="max-width: 500px;" align='center'>
  <table border='1' style='border: 1px solid #ddd; border-collapse: collapse;'>
    <tr>
      <td>
       <img src="./images/TypescriptLogo.svg" width="80" alt="typescript logo"/>
      </td>
      <td>
      <img src="./images/NodeJsLogo.svg" width="80" alt="nodejs logo"/>
      </td>
      <td>
        <img src="./images/ExpressJsLogo.svg" width="80" alt="espressjs logo"/>
      </td>
      <td>
        <img src="./images/mongoDBLogo1.svg" width="80" alt="mongodb logo" />
      </td>
      <td>
        <img src="./images/mongooseLogo1.svg" width="80" alt="mongoose logo" />
      </td>
    </tr>
  </table>
  </div>
  
## 📥 Installation
To install this server project into your local machine, first clone the repository from GitHub
```bash
  git clone https://github.com/Moh-RAIEAN/first-website/edit/main/README.md
```

Install install project dependencies with npm
```bash
  cd ./BlogApp
  npm i
```
## ⚙ Configurations
In your root directory, create a .env file and include env variables:-
```bash
  PORT=5000
  NODE_ENV=development
  DATABASE_URL=mongodb+srv://your_database_url/BlogApp
  BCRYPT_SALT_ROUNDS=10
  JWT_ACCESS_TOKEN_SECRET=an_access_token_sceret
  JWT_REFRESH_TOKEN_SECRET=a_refresh_token_sceret
  JWT_ACCESS_TOKEN_EXPIRES_IS=50d
  JWT_REFRESH_TOKEN_EXPIRES_IN=10d
```
