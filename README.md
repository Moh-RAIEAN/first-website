<div align="center">
  <div>
  <img src="./images/BlogLogo.svg" />
  </div>
</div>

# Blog Application Server
The Blog App is a backend for a blogging platform where users can write, update, and delete their blogs. The system will have two roles: Admin and User. The Admin has special permissions to manage users and their blogs, while users can perform CRUD operations on their own blogs. The backend will include secure authentication, role-based access control, and a public API for viewing blogs with search, sort, and filter functionalities.
## 🔬 Used Technologies
<div style="max-width: 500px;" align='center'>
  <table  style='border: 1px solid #ddd; border-collapse: collapse;'>
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
  cd ./cloned/BlogApp
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
## ⚡ How to run?
To run this application in development mode, run this command
```bash
  npm run start:dev
```
To run this application in production mode, first build the application with this command
```bash
  npm run build
```
Start the server in production mode
```bash
  npm run start:prod
```
## 🚏 API endpoints
### Public routes
Create a user:- /api/auth/register (post) <br/>
Login a user:- /api/auth/login (post)<br/>
Get all blogs:- /api/blogs?search=technology&sortBy=createdAt&sortOrder=desc&filter=60b8f42f9c2a3c9b7cbd4f18 (get)<br/>
### User routes
Create a blog:- /api/blogs (post)<br/>
Update a blog:- /api/blogs/:id (patch)<br/>
Delete a blog:- /api/blogs/:id (delete)<br/>
### Admin routes
Block a user:- /api/admin/users/:userId/block (patch)<br/>
Delete a blog as admin:- /api/admin/blogs/:id (delete)<br/>
