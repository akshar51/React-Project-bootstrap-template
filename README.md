# React E-Commerce Application – File Documentation

---

## 📄 `main.jsx`

### Purpose:
Entry point of the React application.

### Description:
- Uses React 18's `createRoot` to render the application.
- Imports:
  - `StrictMode` from React for development checks.
  - `createRoot` from React DOM.
  - Main `App` component.
  - Bootstrap CSS.



## 📄 `App.jsx`

### Purpose:
Defines the main layout and structure of the e-commerce homepage.

---

### Key Sections:

- **SVG Icons**  
  Defines a library of reusable SVG symbols (user, heart, cart, search, etc.).

- **Preloader**  
  Empty placeholder for a loading animation (likely styled via CSS).

- **Offcanvas Panels**  
  - Cart panel with static items and checkout button.  
  - Search panel with an input field and submit button.

- **Header**  
  - Logo section with an image.  
  - Search bar with category selector.  
  - Contact support information.  
  - Icons for user profile, wishlist, and cart (responsive design with offcanvas toggles).

- **Navigation Menu**  
  - Offcanvas-based Bootstrap navbar.  
  - Dropdown menu for extra pages (About, Shop, Blog, etc.).

- **Hero Banners**  
  - Swiper carousel with promotional content and product images.

- **Category Carousel**  
  - Swiper-based slider with category thumbnails (e.g., Fruits, Breads, Drinks).

- **Newly Arrived Brands**  
  - Horizontal swiper of product cards (images + titles).

- **Trending Products Section**  
  - Bootstrap tabs (All, Fruits & Veges, Juices).  
  - Grid layout of product cards with:  
    - Image, title, rating, price  
    - Quantity selector  
    - Add to Cart link  
    - Wishlist button

---

### Technologies Used:
- React  
- Bootstrap 5  
- Swiper.js  
- SVG Sprites for icons  
- Responsive Design

---

### Notes:
- Static data used for product listing and cart.  
- UI is modular and can be converted into reusable React components.  
- No use of React state or dynamic updates yet.


### Code Summary:
```jsx
import { StrictMode } from 'react';
import { createRoot } from 'react-dom/client';
import App from './App.jsx';
import 'bootstrap/dist/css/bootstrap.min.css';

createRoot(document.getElementById('root')).render(
  <StrictMode>
    <App />
  </StrictMode>
);

