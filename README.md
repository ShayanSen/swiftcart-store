# SwiftCart

A full-stack PERN e-commerce application along with customer support feature, built to explore modern web development concepts including authentication, payments, real-time communication, image management and cloud deployment.

## Live Demo

🔗 Live Application: https://swiftcart-store.onrender.com

> For the best experience, please open the application in a desktop browser.

### Demo Video

🔗 https://youtu.be/CrmuIbUKvgQ?si=Itv91UYPswzpT5Xy

---

## Project Overview

SwiftCart is an online shopping platform where users can browse products, manage their cart, place orders, complete payments and communicate with support through real-time chat and video calls.
The project was built as a learning-focused full-stack application using the PERN stack and several modern developer tools.

---

## Features

### Customer Features

- User authentication and account management
- Browse products by category
- Product catalog with responsive design
- Add and manage cart items
- Secure checkout process
- Order history tracking
- Real-time support chat
- Video call support for order assistance

### Admin Features

- Product management
- Inventory management
- Order monitoring
- Support workflow management

---

## Tech Stack

### Frontend

- React
- Vite
- Tailwind CSS
- DaisyUI
- React Query
- Zustand

### Backend

- Node.js
- Express.js
- TypeScript

### Database

- PostgreSQL
- Drizzle ORM
- Neon Database

### Authentication

- Clerk

### Payments

- Polar

### Media Storage

- ImageKit

### Real-Time Communication

- Stream Chat
- Stream Video

### Monitoring

- Sentry

### Deployment

- Docker
- Render

## Detailed Folder Structure

```
swiftcart-store/
│
├── backend/
│   ├── scripts/
│   │   └── seed.ts
│   │
│   ├── src/
│   │   │
│   │   ├── controllers/
│   │   │   ├── adminController.ts
│   │   │   ├── checkoutController.ts
│   │   │   ├── orderController.ts
│   │   │   ├── productController.ts
│   │   │   └── streamController.ts
│   │   │
│   │   ├── db/
│   │   │   ├── index.ts
│   │   │   └── schema.ts
│   │   │
│   │   ├── lib/
│   │   │   ├── cron.ts
│   │   │   ├── env.ts
│   │   │   ├── imagekit.ts
│   │   │   ├── polar.ts
│   │   │   ├── roles.ts
│   │   │   ├── stream.ts
│   │   │   └── users.ts
│   │   │
│   │   ├── middleware/
│   │   │   └── sentryClerkUser.ts
│   │   │
│   │   ├── routes/
│   │   │   ├── adminRouter.ts
│   │   │   ├── checkoutRouter.ts
│   │   │   ├── meRouter.ts
│   │   │   ├── orderRouter.ts
│   │   │   ├── productRouter.ts
│   │   │   └── streamRouter.ts
│   │   │
│   │   ├── webhooks/
│   │   │   ├── clerk.ts
│   │   │   └── polar.ts
│   │   │
│   │   ├── index.ts
│   │   └── instrument.ts
│   │
│   ├── .env.example
│   ├── drizzle.config.ts
│   ├── package.json
│   ├── package-lock.json
│   └── tsconfig.json
│
├── frontend/
│   │
│   ├── assets/
│   │   ├── favicon.svg
│   │   └── icon.svg
│   │
│   ├── public/
│   │
│   ├── src/
│   │   │
│   │   ├── components/
│   │   │   ├── AdminProductForm.jsx
│   │   │   ├── CatalogProductCard.jsx
│   │   │   ├── EmptyCart.jsx
│   │   │   ├── Footer.jsx
│   │   │   ├── HomeHero.jsx
│   │   │   ├── Layout.jsx
│   │   │   ├── LoadingSkeleton.jsx
│   │   │   ├── Navbar.jsx
│   │   │   ├── OrderPreview.jsx
│   │   │   ├── PageError.jsx
│   │   │   ├── PageLoader.jsx
│   │   │   ├── SentryErrorFallback.jsx
│   │   │   ├── SentryUserSync.jsx
│   │   │   └── TrustStrip.jsx
│   │   │
│   │   ├── hooks/
│   │   │   ├── useAdminProductsPage.js
│   │   │   ├── useCartPage.js
│   │   │   ├── useHomeCatalog.js
│   │   │   ├── useOrderChatPage.js
│   │   │   ├── useOrderDetailPage.js
│   │   │   ├── useOrdersPage.js
│   │   │   ├── useOrderVideoPage.js
│   │   │   └── useProductPage.js
│   │   │
│   │   ├── lib/
│   │   │   ├── api.js
│   │   │   ├── imagekitUpload.js
│   │   │   └── imagekitUrl.js
│   │   │
│   │   ├── pages/
│   │   │   ├── AdminProductsPage.jsx
│   │   │   ├── CartPage.jsx
│   │   │   ├── CheckoutReturnPage.jsx
│   │   │   ├── HomePage.jsx
│   │   │   ├── OrderChatPage.jsx
│   │   │   ├── OrderDetailPage.jsx
│   │   │   ├── OrdersPage.jsx
│   │   │   ├── OrderSummaryPage.jsx
│   │   │   ├── OrderVideoPage.jsx
│   │   │   ├── ProductDetailPage.jsx
│   │   │   └── SentryDemoPage.jsx
│   │   │
│   │   ├── store/
│   │   │   └── cart.js
│   │   │
│   │   ├── utils/
│   │   │   └── format.js
│   │   │
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   │
│   ├── .env
│   ├── .gitignore
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── README.md
│   └── vite.config.js
│
├── .dockerignore
├── .gitignore
├── Dockerfile
└── README.md
```

## Home Page
<img width="1599" height="849" alt="demo_img1" src="https://github.com/user-attachments/assets/74890cd5-f778-4668-9fed-f1efb9f51c19" />
<img width="1599" height="849" alt="demo_img6" src="https://github.com/user-attachments/assets/a089c4da-8cb5-4794-bdb9-c164061842c3" />

## Authentication Page 
<img width="1920" height="1020" alt="demo_img2" src="https://github.com/user-attachments/assets/f28d232f-f833-4e37-aae1-1431759568fc" />
<img width="1920" height="1020" alt="demo_img3" src="https://github.com/user-attachments/assets/93bff0fd-43b0-4aa2-a8ab-953e417731ba" />
<img width="1599" height="849" alt="demo_img4" src="https://github.com/user-attachments/assets/9f5e8fc7-ad24-4941-82d0-163972912818" />

## Empty Cart Page 
<img width="1920" height="1020" alt="demo_img5" src="https://github.com/user-attachments/assets/c78e1f72-7cbc-4ea1-a3d3-20a2cb1ea09f" />

## Product Details Page 
<img width="1599" height="849" alt="demo_img7" src="https://github.com/user-attachments/assets/81e49f9e-4b13-47d7-b910-edd147cbd4a5" />

## Product Catalog / Categories Page 
<img width="1599" height="849" alt="demo_img8" src="https://github.com/user-attachments/assets/0eee3aae-0e4c-4a2f-a31c-35cde3fa2ca3" />
<img width="1920" height="1020" alt="demo_img9" src="https://github.com/user-attachments/assets/53ef7192-7001-4057-8a4e-041287ee5b37" />
<img width="1599" height="849" alt="demo_img10" src="https://github.com/user-attachments/assets/f20a608c-0ad6-4b37-baa9-aeaaf972beef" />
<img width="1920" height="1020" alt="demo_img11" src="https://github.com/user-attachments/assets/9963af47-82bb-4cd7-9e59-78cd8faf2656" />
<img width="1920" height="1020" alt="demo_img12" src="https://github.com/user-attachments/assets/edcd9842-d86c-4b4a-9874-dd1cb535808d" />
<img width="1599" height="849" alt="demo_img13" src="https://github.com/user-attachments/assets/4183943c-bc85-4f31-b85a-8416b787b8a6" />

## Shopping Cart Page 
<img width="1920" height="1020" alt="demo_img14" src="https://github.com/user-attachments/assets/c0b38249-91c6-4ca5-a0bb-a260c08c8198" />
<img width="1599" height="849" alt="demo_img15" src="https://github.com/user-attachments/assets/308c74c6-90c2-43e4-9755-95caf3849e78" />
<img width="1920" height="1020" alt="demo_img16" src="https://github.com/user-attachments/assets/bfb21112-ca0a-4ca5-930d-0dac56827c61" />

## Checkout / Payment Page 
<img width="1920" height="1020" alt="demo_img17" src="https://github.com/user-attachments/assets/d9f87121-71a1-4ed1-9610-cdff41f7e9d2" />

## Order Confirmation Page 
<img width="1920" height="1020" alt="demo_img18" src="https://github.com/user-attachments/assets/802643b6-6329-44a3-9f97-81692ae327ea" />

## Orders Page 
<img width="1920" height="1020" alt="demo_img19" src="https://github.com/user-attachments/assets/ce7aa480-305b-4f67-a0d7-ee46c86c7eef" />

## Order Details Page (nested Order Summary Page)
<img width="1920" height="1020" alt="demo_img20" src="https://github.com/user-attachments/assets/033f43d8-cb4e-4ad9-8ea9-e34479fc4289" />

## Order Details Page (nested Support Chat Page)
<img width="1920" height="1020" alt="demo_img21" src="https://github.com/user-attachments/assets/4c3c2d71-70b6-4bd1-8c09-18f5152f6e5e" />

## Video Support Page 
<img width="1920" height="1020" alt="demo_img22" src="https://github.com/user-attachments/assets/26f3f433-59c3-41f4-87b4-4eff07663f4a" />

## Admin Products Management Page 
<img width="1920" height="1020" alt="demo_img23" src="https://github.com/user-attachments/assets/53f60975-522d-4861-927d-1f58a6b5e68a" />
<img width="1920" height="1020" alt="demo_img24" src="https://github.com/user-attachments/assets/abad567e-2d11-43b5-a49b-bd1e3b797133" />

## Order & Account Email Notifications  
<img width="1920" height="1020" alt="demo_img25" src="https://github.com/user-attachments/assets/fa272dba-14d1-4d7b-b61b-9a100caff5df" />


