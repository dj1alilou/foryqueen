# ForyQueen - Jewelry E-commerce

A beautiful jewelry e-commerce website built with Node.js, Express, MongoDB, and Cloudinary.

## Features

- 🛍️ Product catalog with categories (Parure, Bracelet, Bague, Boucles, Montre, Collier)
- 🛒 Shopping cart with quantity management
- 📱 Responsive design for mobile and desktop
- 📦 Order management system
- 📊 Admin dashboard
- ☁️ Cloudinary for image storage
- 🗂️ MongoDB database (or file-based fallback)

## Tech Stack

- **Backend**: Node.js + Express
- **Database**: MongoDB Atlas (or file-based storage)
- **Image Storage**: Cloudinary
- **Frontend**: HTML, CSS, JavaScript (Tailwind CSS)
- **Deployment**: Vercel (frontend), Render (backend)

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/foryqueen.git
cd foryqueen
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Copy the `.env.example` file to `.env` and fill in your values:

```bash
cp .env.example .env
```

Edit `.env` with your settings:

- **MONGODB_URI**: Your MongoDB Atlas connection string
- **CLOUDINARY_CLOUD_NAME**: Your Cloudinary cloud name
- **CLOUDINARY_API_KEY**: Your Cloudinary API key
- **CLOUDINARY_API_SECRET**: Your Cloudinary API secret
- **PORT**: Server port (default: 4000)

### 4. Run locally

```bash
npm start
```

Visit http://localhost:4000 for the store and http://localhost:4000/admin for the admin dashboard.

## Deployment

### Backend (Render)

1. Create a new Web Service on Render
2. Connect your GitHub repository
3. Set the following:
   - Build Command: (empty)
   - Start Command: `node server.js`
   - Environment Variables: Add all variables from your `.env` file

### Frontend (Vercel)

1. Import your project to Vercel
2. Set the following:
   - Build Command: (empty)
   - Output Directory: (empty)
   - Install Command: (empty)

Or use the included `vercel.json` configuration.

## Project Structure

```
foryqueen/
├── server.js          # Main server file
├── index.html         # Customer-facing store
├── admin.html         # Admin dashboard
├── admin.js           # Admin JavaScript
├── index.js           # Store JavaScript
├── package.json       # Dependencies
├── vercel.json        # Vercel configuration
├── ping.js            # Health check script
├── .env.example       # Environment variables template
├── data/
│   ├── products.json  # Products data (fallback)
│   └── orders.json    # Orders data (fallback)
├── images/            # Static images
└── uploads/           # Temporary uploads
```

## License

MIT License
