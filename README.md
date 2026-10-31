# ShareBite - Surplus Food Rescue & Community Donation Platform

A clean, responsive food rescue web application built with **React**, **Tailwind CSS**, and **Lucide Icons**. ShareBite connects restaurants, bakeries, and caterers with local NGOs and community food banks to minimize food waste and alleviate hunger.

---

## 🌟 Key Features

### 1. 🔄 Multi-Role Architecture (Top Header Switcher)
- **Donor (Restaurant / Caterer)**: Manage surplus kitchen donations, accept or reject incoming NGO collection requests, and track meals shared.
- **Recipient (NGO / Charity)**: Search available surplus food, request urgent pickups, and track rescue operations with a 3-step live status stepper.
- **Admin (Moderation & Safety)**: Moderate platform listings with 1-click flag/remove actions, view compliance logs, and review verified NGO / donor profiles.
- **Contextual Persona Picker**: Seamlessly switch between 4 donor restaurants and 3 registered NGOs to test multi-party interactions in real-time.

### 2. 🍲 Donor Dashboard
- **'Donate Food' Modal Form**:
  - Title & Category selection (`Cooked Meals`, `Raw Produce`, `Packaged Goods`)
  - Dietary classification (`Vegetarian`, `Vegan`, `Non-Veg Halal`, `Gluten-Free`)
  - Exact Quantity (units/weight) and estimated portions served
  - Preparation / Cooked time & Safe use-by window countdown
  - Pickup location & Landmark notes
  - Special handling instructions (thermal insulation, strict refrigeration, allergen tags)
  - Mandatory food safety compliance check
- **Listings Management**:
  - Status pills: `Available`, `Requested`, `Accepted`, `Completed`, `Flagged`
  - Real-time action cards for pending requests: **Accept Pickup** or **Decline / Reject** (with reason modal).
  - Metrics: Meals Shared, Active Listings, Pending Requests, CO2 Emissions Prevented.

### 3. 🤝 Recipient / NGO Portal
- **Surplus Food Feed**:
  - Instant search across food items, restaurants, and neighborhoods
  - Category filters (`Cooked`, `Packaged`, `Raw`) and Dietary filters (`Veg`, `Vegan`, `Non-Veg`)
  - Dynamic urgency badges (e.g. `Urgent: 3.5h safe`)
- **Request Pickup Confirmation Modal**:
  - Select active NGO identity (e.g. Robin Hood Army, Hope & Hunger Mission, City Youth Shelter)
  - Volunteer arrival ETA selection (e.g. 20-30 mins, 45 mins)
  - Transport & cooling equipment specification
  - Direct coordinator phone number
- **'My Requests' Tracking Tab**:
  - Live 3-Stage Stepper: `1. Pending` ➔ `2. Accepted` ➔ `3. Picked Up / Completed`
  - **Digital Pickup Pass**: Generates official authorization voucher with QR code, verification PIN, temperature handover checklist, and 1-click "Mark as Picked Up".

### 4. 🛡️ Admin Moderation & Food Safety Center
- High-level KPIs: Total Listings, Active Surplus, Rescued Portions, Verified Charities, Flagged Listings.
- **1-Click Moderation**: Flag/Remove listings with violation categorization (`Danger Zone temperature breach`, `Expired window`, etc.) and instant 1-Click Restore.
- **Food Safety & Good Samaritan Liability Disclaimer Banner**: Explains civil and criminal liability protection under 42 U.S. Code § 1791 (Bill Emerson Act) and temperature guidelines (≥60°C or ≤4°C).
- Chronological real-time platform Audit Log.

### 5. 📦 Preloaded Realistic Mock Data
- **11 Pre-populated Listings**:
  - *Hyderabadi Dum Biryani Handi (30 portions)*
  - *Fresh Artisan Sourdough & Multigrain Bread (15 loaves)*
  - *Surplus Banquet Buffet Curries & Steamed Basmati (50 meals)*
  - *Organic Farm-Fresh Spinach & Tomatoes (18 kg)*
  - *Pasteurized Whole Milk & Greek Yogurt Cartons (40 units)*
  - *Gourmet Woodfired Neapolitan Pizzas (12 large pies)*
  - *Assorted Deli Sandwiches & Healthy Wraps (35 packs)*
  - *Steamed Dim Sum, Bao Buns & Noodles (20 portions)*
  - *Fresh Fruit Platter Trays (15 boxes)*
  - *Breakfast Pastries & Croissants (28 pcs)*
  - *Farm Surplus Potatoes & Carrots (35 kg)*
- **3 Registered NGO Profiles** with verified 501(c)(3) IDs, vehicle fleets, ratings, and contacts:
  1. *Robin Hood Army - Central Chapter*
  2. *Hope & Hunger Relief Mission*
  3. *City Youth & Shelter Foundation*
- **4 Registered Donor Kitchens**:
  1. *The Royal Biryani House*
  2. *Artisan Oven Bakery & Cafe*
  3. *Grand Palace Caterers & Events*
  4. *Green Earth Farm to Table*

### 6. ⚡ Live Multi-Tab LocalStorage Persistence
- All listing creation, pickup requests, acceptance, handovers, and admin flags persist in `localStorage` and synchronize live across multiple browser tabs via `storage` event listeners.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm

### Installation & Running Locally
```bash
# Navigate to the project directory
cd sharebite

# Install dependencies (already pre-installed)
npm install

# Run the development server
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

