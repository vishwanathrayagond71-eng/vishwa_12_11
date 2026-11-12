# vishwa_12_11
Tours and Tour 🌍✈️
A professional, modern, and fully responsive tourism website built with Node.js, Express, EJS, CSS, and Vanilla JavaScript. It uses Excel sheets (.xlsx) as a lightweight database, meaning no MongoDB or SQL installation is required!

🌟 Key Features
User Authentication & Dashboard:
Register, login, and logout.
Profile management and history of bookings and reviews.
Secure password hashing with bcryptjs.
Interactive UI/UX:
Custom-built interactive hero slider, smooth animations, and scroll reveal.
Dedicated destinations & packages pages with search, filtering, and wishlist features (persisted in LocalStorage).
Star-rating review system, dynamic contact page with Google Maps embed, and FAQ accordion.
Integrated Travel Bot (Chatbot) with a comprehensive local knowledge base and quick-reply buttons.
Light & Dark mode toggle with automatic preference preservation.
Excel-based Database Engine:
Instead of SQL/MongoDB, all user registrations, packages booking, reviews, contact inquiries, and newsletter signups are written dynamically in Excel files.
Stored structured tables inside excel-data/ folder.
Interactive Admin Panel:
Dedicated dashboard at /admin/login.
Admin stats cards showing total users, bookings, revenue, and reviews.
View, search, and delete records (Users, Bookings, Reviews, Contacts, Newsletters).
One-click direct Excel download for all 5 databases directly from the dashboard!
📂 Project Structure
├── excel-data/             # Auto-generated Excel sheets (users, bookings, etc.)
├── middleware/
│   └── auth.js             # Authentication checks (user/admin login validations)
├── public/
│   ├── css/
│   │   └── style.css       # Custom stylesheets (Light/Dark design system)
│   └── js/
│       ├── main.js         # Interactive main script, animations, wishlist
│       └── chat.js         # Chatbot bot widget client logic
├── routes/
│   └── index.js            # Express routes (pages, auth logic, actions, data)
├── utils/
│   └── excelService.js     # Excel database interface wrapper
├── views/
│   ├── partials/
│   │   ├── header.ejs      # Scripts/meta tags (shared headers)
│   │   ├── navbar.ejs      # Dynamic navigation (auth, theme switcher)
│   │   └── footer.ejs      # Custom footer, chatbot, scripts loading
│   ├── 404.ejs             # Not Found Page
│   ├── about.ejs           # Company story, team, FAQs
│   ├── admin-dashboard.ejs # Responsive Admin Panel
│   ├── admin-login.ejs     # Admin login screen
│   ├── booking.ejs         # Multi-step checkout form
│   ├── contact.ejs         # Contact forms & map details
│   ├── dashboard.ejs       # User account details
│   ├── destinations.ejs    # Destination explorer
│   ├── home.ejs            # Main landing page
│   ├── login.ejs           # Sign-in portal
│   ├── packages.ejs        # Available packages catalog
│   ├── register.ejs        # Account registration
│   └── reviews.ejs         # Guest feedback board
├── .env                    # Secrets and environment configs
├── server.js               # Application bootstrap file
└── package.json            # Node dependency configuration
