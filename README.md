# plant-nursery-system

Plant Nursery E-commerce System prototype featuring:  

- **Seller Registration**: sellers can sign up, login, and list plants.  
- **Customer Cart System**: customers can browse, add to cart, and checkout.  
- **Admin Dashboard**:  
  - Accept/reject online payments  
  - View number of registered users & sellers  
  - Track total purchases & sales  
- **Billing**: create a bill after payment (downloadable in **PDF** format).  
- **Dummy Payment System (Razorpay)** integration.  
- **Login/Logout** mechanism for both customer and seller.  
  - Customers **must login** before buying (system forces login).  
- **Seller Dashboard**: shows how many products a seller has sold and how much they earned.  

**Backend:** Node.js + JSON  
**Frontend:** HTML, CSS, JavaScript  

---

## 🚀 Features

- Seller registration & login  
- Customer login and cart system  
- Admin approval/rejection of payments  
- PDF bill generation after successful payment  
- Razorpay dummy payment system integration  
- Seller dashboard to track earnings & sales  

---

## ⚙️ Razorpay Setup

Before setting up the Razorpay dummy payment system:  

1. Create your own Razorpay **key_id** and **key_secret** from the Razorpay Dashboard.  
2. Replace them in `server.js`:  

   ```js
   const razorpay = new Razorpay({
     key_id: 'rzp_test_btop9zW7LAr6UC',
     key_secret: 'FYMersDitnfb0lORO9bm4zqs'
   });
#👉 Replace both values with your test keys.

#Run the server locally:

bash
Copy code
node server.js
Use ngrok to expose your local server:

bash
Copy code
ngrok http 3000
This will give you a valid HTTPS link for your locally running app.
Use this link to configure Razorpay’s test checkout and callbacks.

#🧪 Tech Stack
Backend: Node.js, JSON

Frontend: HTML, CSS, JavaScript

Payments: Razorpay (Dummy Test Mode)

Tunnel: ngrok (to expose localhost)

