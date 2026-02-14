# 💧 AquaStore - Water Can & Bulk Water Delivery Frontend

A complete Flipkart-style water delivery e-commerce platform built with pure HTML, CSS, and JavaScript using Bootstrap 5.

## 🎨 Features

- **Modern UI**: Clean, responsive design with Bootstrap 5
- **Water Theme**: Blue gradient color scheme (#007BFF, #00CFFF)
- **Sticky Navigation**: Always accessible navbar with cart badge
- **Product Management**: Browse, filter, and sort water products
- **Shopping Cart**: Add/remove items, quantity controls
- **Mandatory Address**: Checkout requires complete address validation
- **Admin Dashboard**: Stock management and order tracking
- **Local Storage**: Persistent cart and user data
- **Form Validation**: Real-time input validation with error messages

## 📁 Project Structure

```
aqua_store_frontend/
│
├── index.html              # Homepage with hero section and featured products
├── product_list.html        # Product listing with filters and sorting
├── product_detail.html       # Individual product details page
├── cart.html              # Shopping cart with quantity controls
├── checkout.html           # Checkout with mandatory address validation
├── login.html             # User login page
├── register.html           # User registration page
├── admin_dashboard.html     # Admin panel for stock and orders
│
├── css/
│   └── style.css          # Custom styles and responsive design
├── js/
│   └── main.js           # Core JavaScript functionality
└── README.md             # This file
```

## 🚀 Quick Start

1. **Open any HTML file** in your browser - no server required!
2. **Start with `index.html`** for the main experience
3. **Navigate** through the application using the menu

## 🔑 Demo Credentials

### User Registration
- Create any account using the registration form
- All fields are required (Username, Email, Password)

### Admin Access
- Direct access to admin dashboard (no authentication required for demo)

## 📱 Pages & Features

### 🏠 Homepage (`index.html`)
- Hero section with gradient background
- Featured water cans (1L, 2L, 5L, 10L, 20L)
- Add to cart functionality
- Dynamic cart badge

### 🛍️ Product Listing (`product_list.html`)
- Grid layout with product cards
- Filter by size (1L, 2L, 5L, 10L, 20L, 50L, 100L, 200L)
- Sort by price (Low to High, High to Low)
- Add to cart and view details

### 📋 Product Detail (`product_detail.html`)
- Large product images
- Detailed descriptions
- Quantity selector (1-10)
- Dynamic price calculation
- Add multiple quantities to cart

### 🛒 Shopping Cart (`cart.html`)
- Item list with images
- Quantity controls (+ / -)
- Individual item totals
- Grand total calculation
- Remove items functionality
- Proceed to checkout

### 📦 Checkout (`checkout.html`)
- **MANDATORY ADDRESS FIELDS**:
  - Full Name (required)
  - Address Line (required)
  - City (required)
  - PIN Code (required, 6-digit validation)
  - Phone Number (required, 10-digit validation)
- Payment methods: Cash on Delivery, Online Payment
- Real-time validation with error messages
- Order processing with success feedback

### 🔐 Authentication
- **Login**: Email and password authentication
- **Register**: Username, email, password registration
- LocalStorage user management

### 🎛️ Admin Dashboard (`admin_dashboard.html`)
- Stock cards for each water can size
- Daily orders table
- Order status management:
  - Placed
  - Confirmed
  - Out for Delivery
  - Delivered
  - Cancelled

## ✅ Validation Features

### Checkout Form Validation:
- **Required Fields**: All address fields must be filled
- **PIN Code**: Exactly 6 digits (regex: /^\d{6}$/)
- **Phone Number**: Exactly 10 digits (regex: /^\d{10}$/)
- **Real-time Validation**: Instant feedback as user types
- **Error Messages**: Clear, inline error display
- **Form Blocking**: Prevents submission if validation fails

### Input Validation:
- HTML5 `required` attributes
- JavaScript regex validation
- Visual feedback with Bootstrap validation classes
- Custom error messages

## 🎨 Design System

### Colors:
- **Primary**: #007BFF (Blue)
- **Secondary**: #00CFFF (Cyan)
- **Success**: #28a745
- **Danger**: #dc3545
- **Warning**: #ffc107

### Components:
- **Cards**: Shadow effects, hover animations
- **Buttons**: Gradient effects, hover states
- **Forms**: Input groups with icons
- **Navigation**: Sticky, responsive
- **Modals**: Bootstrap 5 modals
- **Badges**: Dynamic cart count

## 📱 Responsive Design

- **Mobile**: Optimized for phones (320px+)
- **Tablet**: Tablet-friendly layouts (768px+)
- **Desktop**: Full desktop experience (1024px+)
- **Touch-friendly**: Large tap targets
- **Flexible Grid**: Bootstrap grid system

## 💾 Data Storage

### LocalStorage Keys:
- `aquaStoreCart`: Shopping cart items
- `aquaStoreUsers`: Registered users
- `aquaStoreCurrentUser`: Logged-in user
- `aquaStoreOrders`: Order history

### Data Structure:
```javascript
// Cart Item
{
  id: 1,
  name: "1L Water Can",
  price: 25,
  image: "url",
  quantity: 2
}

// Order
{
  orderId: "ORD1234567890",
  fullName: "John Doe",
  address: "123 Street",
  city: "Mumbai",
  pincode: "400001",
  phone: "9876543210",
  paymentMethod: "Cash on Delivery",
  totalAmount: 250,
  items: [...],
  status: "Placed"
}
```

## 🔧 Technical Features

### JavaScript Functions:
- **Cart Management**: Add, remove, update quantities
- **Form Validation**: Real-time validation with regex
- **Storage**: LocalStorage persistence
- **Notifications**: Success/error messages
- **Dynamic Updates**: Cart badge, totals
- **Order Processing**: Complete checkout flow

### CSS Features:
- **Animations**: Smooth transitions, hover effects
- **Gradients**: Blue gradient backgrounds
- **Responsive**: Mobile-first design
- **Custom Scrollbar**: Styled scrollbar
- **Loading States**: Spinner animations

## 🌐 Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers

## 🚀 Deployment

### Static Hosting:
- Netlify
- Vercel
- GitHub Pages
- Firebase Hosting
- Any static file server

### Local Development:
```bash
# Simple HTTP server
python -m http.server 8000

# Node.js server
npx serve .

# Live Server
npx live-server
```

## 📋 Key Features Summary

### ✅ Implemented:
- [x] Complete product catalog
- [x] Shopping cart with localStorage
- [x] Mandatory address validation
- [x] Form validation with regex
- [x] Admin dashboard
- [x] Responsive design
- [x] Modern UI with Bootstrap 5
- [x] LocalStorage persistence
- [x] Real-time validation
- [x] Order management
- [x] Stock management UI

### 🔄 Ready for Backend:
- User authentication API
- Product management API
- Order processing API
- Payment gateway integration
- Real stock management
- Email notifications

---

**Built with ❤️ using pure web technologies**
