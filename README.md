# ✅ Task Manager App

> A simple full-stack app to manage daily tasks.  
> Track, update, and complete tasks with ease.  
> Task management made easy with Node and React.  
> A lightweight MERN-based task tracker.  
> Manage your to-dos in a clean, responsive interface.  
> A JWT-authenticated app to create and manage tasks.

---

## 🔧 Requirements

- **Node.js**: v23.10.0  
- **npm**: v11.2.0  
- **MongoDB Atlas** account  

---

## 🚀 Getting Started

### 🔙 Backend (Express.js)

1. Open your terminal and navigate to the `backend` folder:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up MongoDB Atlas:

   - Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
   - Create an account and log in
   - Click **"New Project"**, enter a name, and click **"Next"**
   - Add members if needed → click **"Create Project"**
   - In the side menu, click **"Clusters"** → **"Build a Cluster"**
   - Choose **Free Tier**, name your cluster, and select a cloud provider/region
   - Click **"Create Cluster"**
   - Whitelist your IP address under **Network Access**
   - Create a database user and password under **Database Access**
   - Click **"Connect"** → choose **"Drivers"** → copy the **Node.js connection string**

4. Configure environment variables:

   In the `backend` folder, create a `.env` file:

   ```env
   MONGO_URI=<your_mongodb_connection_string>
   JWT_SECRET=<your_generated_jwt_secret>
   ```

   > Replace `<password>` in the connection string with your actual DB password.

   To generate a strong JWT secret:

   ```bash
   node -e "console.log(require('crypto').randomBytes(64).toString('hex'))"
   ```

5. Start the backend server:

   ```bash
   npm run dev
   ```

---

### 🖥️ Frontend (React)

1. In a new terminal, navigate to the frontend directory:

   ```bash
   cd frontend/Task-Manager
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

   Your app should now be running at [http://localhost:5173](http://localhost:5173) (or the default Vite port).

---

## 📁 Project Structure

```bash
root
├── backend              # Express.js backend with REST APIs
│   └── .env             # Environment configuration
├── frontend
│   └── Task-Manager     # React frontend (Vite-based)
```



