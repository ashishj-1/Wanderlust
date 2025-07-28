# 🌍 Wanderlust

**Wanderlust** is a full-stack travel and property listing web application inspired by Airbnb.
It allows users to register, log in, create listings, leave reviews, and explore accommodations worldwide — with support for location-based search using Mapbox.

🔗 **Live Website:** [Wanderlust on Render](https://airbnb-clone-97nf.onrender.com/listings)

---

# ✨ Features

- 🔐 User authentication and session management with Passport.js
- 🏠 Full CRUD for property listings
- ⭐ Review and rating system for listings
- 📍 Location-based listings using **Mapbox Geocoding API**
- 🌐 Deployed on **Render**
- 📮 API validation and testing using **Postman**
- 🧠 Robust error handling with custom middleware
- 🧰 Organized MVC structure with separate controllers, routes, models, and utilities
  
---

# 🛠 Tech Stack

| Layer             | Technology                             |
|------------------|-----------------------------------------|
| Frontend          | EJS, CSS, Bootstrap                    |
| Backend           | Node.js, Express.js                    |
| Database          | MongoDB Atlas                          |
| Authentication    | Passport.js, express-session           |
| Geocoding         | Mapbox Geocoding API                   |
| Dev Tools         | dotenv, method-override, connect-flash |
| Deployment        | Render                                 |
| API Testing       | Postman                                |

---

# 📁 Folder Structure

```

Wanderlust/
├── controllers/        # Logic for listings, reviews, and auth
├── init/               # Initial configuration files
├── models/             # Mongoose models (User, Listing, Review)
├── public/             # Static files (CSS, images, JS)
├── routes/             # Modular Express routes
├── utils/              # Custom utilities like ExpressError
├── views/              # EJS templates
├── app.js              # Main application entry point
├── cloudConfig.js      # Cloudinary or other cloud services (future use)
├── middleware.js       # Custom middleware
├── schema.js           # Joi validation schemas
├── .env                # Environment variables (not committed)
├── .gitignore
├── package.json
└── README.md

````

---

# ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/ashishj-1/Wanderlust.git
   cd Wanderlust
``

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   Create a `.env` file in the root:

   ```env
   ATLASDB_URL=your_mongodb_connection_string
   SECRET=your_secure_session_secret
   MAPBOX_TOKEN=your_mapbox_token
   ```

4. **Start the development server**

   ```bash
   node app.js
   ```

   The app will be running on: [http://localhost:8080](http://localhost:8080)

---

# 🌐 Deployment (Render)

To deploy Wanderlust on **Render**:

1. Push the code to GitHub.
2. Go to [https://render.com](https://render.com) → Create New Web Service.
3. Connect your GitHub repository.
4. Set the environment variables:

   * `ATLASDB_URL`
   * `SECRET`
   * `MAPBOX_TOKEN`
5. Build Command: `npm install`
6. Start Command: `node app.js`
7. Deploy!

---

# 🧪 API Testing with Postman

You can use **Postman** to test all the main API routes.

| Method | Route                        | Description       |
| ------ | ---------------------------- | ----------------- |
| POST   | `/register`                  | User registration |
| POST   | `/login`                     | User login        |
| GET    | `/listings`                  | View all listings |
| POST   | `/listings`                  | Create a listing  |
| PUT    | `/listings/:id`              | Update a listing  |
| DELETE | `/listings/:id`              | Delete a listing  |
| POST   | `/listings/:id/reviews`      | Add a review      |
| DELETE | `/listings/:id/reviews/:rid` | Delete a review   |

> Optional: Attach a Postman collection in the repo for testing ease.

---

# 📍 Mapbox Integration

Wanderlust uses **Mapbox Geocoding API** to convert user-entered location names into coordinates (latitude & longitude), enabling smart location-based listings.

Configure it in `.env`:

```env
MAPBOX_TOKEN=your_mapbox_access_token
```

---

# 📸 Screenshots (Optional)

> Include screenshots of:
> * Homepage
<img width="1920" height="1080" alt="Screenshot 2025-07-28 143616" src="https://github.com/user-attachments/assets/29b21ab0-75c8-4040-991d-7a97363cc854" />

> * Listing page
<img width="1920" height="1080" alt="Screenshot 2025-07-28 144502" src="https://github.com/user-attachments/assets/f58e488f-3424-498f-99ad-12cdc6cd6b15" />

> * Review section
<img width="1185" height="778" alt="Screenshot 2025-07-28 144111" src="https://github.com/user-attachments/assets/ba7b4885-30a8-4332-8088-af68efc22719" />

> * Authentication (register/login)
<img width="1920" height="1080" alt="Screenshot 2025-07-28 143703" src="https://github.com/user-attachments/assets/8cd771fd-b6c7-481a-9ec7-54ad0286fc59" />
<img width="1920" height="1080" alt="Screenshot 2025-07-28 143717" src="https://github.com/user-attachments/assets/cf7fc853-73a0-420e-af69-cf895878f3d8" />
---

> * Listed Property
<img width="1150" height="687" alt="Screenshot 2025-07-28 143822" src="https://github.com/user-attachments/assets/b3d056b7-ce0c-44ea-a977-f32c6bd23dce" />
> * Mapbox integration
<img width="992" height="467" alt="Screenshot 2025-07-28 143838" src="https://github.com/user-attachments/assets/209f08ed-9b1e-4c67-ab63-92e134353d6e" />


# 📄 License

This project is licensed under the **MIT License**.

---

# 🙏 Acknowledgements

* [Mapbox](https://www.mapbox.com/)
* [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
* [Render](https://render.com)
* [Postman](https://www.postman.com)
````
