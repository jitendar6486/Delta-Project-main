# 🏕️ Wanderlust - Travel Listing App

Wanderlust is a full-featured travel listing web application built with **Node.js**, **Express**, **MongoDB**, and **EJS**. It allows users to sign up, log in, create, edit, and review listings for travel destinations. It also integrates with **Cloudinary** for image uploads and **Mapbox** for geolocation services.

---

## 🚀 Features

- 🧭 Create, edit, delete travel listings
- 💬 Add reviews and ratings for each listing
- 🖼️ Upload images via Cloudinary
- 🗺️ Geolocation and maps with Mapbox
- 🔐 Authentication using Passport.js
- 🌐 Flash messages for user feedback
- 🧱 Modular MVC architecture

---

## 🛠️ Project Structure
📦 Delta-Project-main
┣ 📂 controllers/ # Route logic
┣ 📂 models/ # Mongoose schemas
┣ 📂 routes/ # Express routes
┣ 📂 views/ # EJS templates
┣ 📂 public/ # Static assets (CSS/JS)
┣ 📂 utils/ # Helper functions
┣ 📂 init/ # Seeding scripts
┣ 📄 app.js # Entry point
┣ 📄 cloudConfig.js # Cloudinary config
┣ 📄 package.json
┣ 📄 .env # Environment variables (not committed)
┣ 📄 .gitignore


---

## 📌 Steps You Followed

### 1. Initialized the Node.js project:

* Ran `npm init` and installed core dependencies like **Express**, **Mongoose**, **EJS**, and **Dotenv**.
* Set up the project structure using the **MVC pattern** for better code organization.

### 2. Built the server using Express (`app.js`):

* Set up routes and middleware including `express-session`, `connect-flash`, `passport`, and `method-override`.
* Configured MongoDB connection using **Mongoose** and `.env` variables for secure credentials.

### 3. Designed dynamic pages using EJS:

* Created clean and reusable **EJS templates** for listings, forms, and authentication pages.
* Used `ejs-mate` for layout support with partials like navbar, footer, and flash messages.

### 4. Implemented user authentication:

* Used **Passport.js** with `passport-local` and `User.authenticate()` for sign up and login.
* Secured user sessions and added flash messaging for login success/failure feedback.

### 5. Developed listing and review features:

* Created models for `Listing`, `Review`, and `User` using Mongoose schemas.
* Set up route controllers to **create, edit, delete, and review listings**.
* Nested routes for adding reviews under specific listings.

### 6. Integrated Cloudinary for image uploads:

* Configured **Cloudinary and multer-storage-cloudinary** to allow users to upload listing images.
* Stored uploaded images in the `wanderlust_DEV` Cloudinary folder.

### 7. Used environment variables securely:

* Managed API keys and database URLs via a `.env` file.
* Ensured `.env` is excluded from the repo using `.gitignore`.

### 8. Handled errors and 404s:

* Created a custom `ExpressError` utility.
* Used a catch-all route (`app.all("*")`) to handle non-existent paths gracefully with a styled error page.

---
## 📦 Technologies Used

- Node.js  
- Express.js  
- MongoDB + Mongoose  
- EJS Templating  
- Passport.js  
- Cloudinary & Multer  
- Mapbox API  
- connect-flash  
- express-session  

---

 **"💻 How to Run Locally"** 

---

## 💻 How to Run Locally

1. **Clone the repository:**

   ```bash
   git clone https://github.com/jitendar6486/MajorProject.git
   cd MajorProject
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root directory with the following content (replace with your actual credentials):

   ```env
   ATLASDB_URL=your_mongodb_connection_url
   CLOUD_NAME=your_cloudinary_cloud_name
   CLOUD_API_KEY=your_cloudinary_api_key
   CLOUD_API_SECRET=your_cloudinary_api_secret
   SECRET=your_session_secret
   ```

4. **Run the development server:**

   ```bash
   node app.js
   ```

5. **Open the app in your browser:**

   Visit:

   ```
   http://localhost:8080
   ```

---

---

## ✅ Conclusion

The **Wanderlust** project showcases how to build a complete full-stack web application using **Node.js**, **Express**, **MongoDB**, and **EJS**. It combines server-side logic, authentication, and third-party service integration (like **Cloudinary** and **Mapbox**) to create a dynamic and user-friendly platform for listing and reviewing travel destinations.



---




