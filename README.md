Vehiql AI Car Marketplace 🚗🤖 Hosted link : .https://vehiql-tau.vercel.app/

Vehiql is a modern, AI-powered car marketplace designed to revolutionize how users discover, explore, and book vehicles. Leveraging cutting-edge AI technology and a scalable full-stack architecture, Vehiql automates car listing creation, streamlines test drive bookings, and delivers a seamless, professional user experience.

🌟 Key Features
AI-Powered Car Management

Automatic Car Detail Extraction: Upload images to extract make, model, year, color, body type, mileage, fuel type, transmission, and price.

Confidence Scoring: AI provides confidence levels (0–1) for extracted details.

Smart Form Population: Automatic filling of listing forms with AI-detected information.

Manual Override: Users can review and edit AI-extracted data.

Advanced Search & Discovery

Multi-criteria filtering: Make, model, price, year, fuel type, body type, transmission.

Instant search results with URL state persistence for bookmarking.

Mobile-friendly filter interface with responsive design.

Test Drive Booking System

Time-slot based bookings with conflict detection.

Admin-controlled status updates: PENDING → CONFIRMED → COMPLETED/CANCELLED/NO_SHOW.

Calendar picker with disabled past dates and closed days.

Admin Panel & Inventory Management

AI-powered or manual car listing.

Bulk operations for managing cars and featured listings.

Advanced analytics: Test drive to sale conversion, inventory tracking.

Image gallery management for multiple high-quality car images.

User Experience Enhancements

Wishlist/saved cars functionality.

EMI calculator with dynamic sliders for loan amount, interest, and tenure.

Responsive, mobile-first design.

Smooth animations, transitions, and accessible UI patterns.

🏗️ Tech Stack

Frontend:

Next.js 15 (App Router)

React 19 + TypeScript/JavaScript

Tailwind CSS + Radix UI for reusable, accessible components

Backend & Database:

PostgreSQL with Prisma ORM (type-safe queries)

Supabase for image storage and authentication

Next.js Server Actions for API endpoints

AI & External Services:

Google Gemini 1.5 Flash for image analysis and car detail extraction

Clerk for authentication & social logins

Arcjet for security and bot protection

Deployment & Tools:

Vercel for hosting & serverless deployment

ESLint & Prettier for code quality

Git & GitHub for version control

📁 Project Structure
ai-car-marketplace/
├── app/                    # Next.js App Router
│   ├── (admin)/            # Admin routes
│   ├── (auth)/             # Authentication routes
│   └── (main)/             # Public user routes
├── components/             # Reusable UI components
├── actions/                # Server actions (API layer)
├── lib/                    # Utilities & configurations
├── hooks/                  # Custom React hooks
└── prisma/                 # Database schema & migrations

🔒 Security & Performance

Multi-layer security: Arcjet + Clerk + middleware route protection.

Input validation & CSRF protection.

Optimized database queries with indexing and caching.

Image optimization with Next.js Image component, WebP support, and lazy loading.

🚀 Usage
1. Clone the repository
git clone https://github.com/<your-username>/vehiql.git
cd vehiql

2. Install dependencies
npm install

3. Setup environment variables

Create .env.local with keys:

DATABASE_URL=your_postgres_connection
CLERK_API_KEY=your_clerk_key
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
GEMINI_API_KEY=your_gemini_key
ARCJET_API_KEY=your_arcjet_key

4. Run migrations
npx prisma migrate dev

5. Run the development server
npm run dev
