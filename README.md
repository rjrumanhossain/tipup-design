# TOPUPBUZZ Frontend Clone

শুধুমাত্র **Frontend Design** ক্লোন। Backend তুমি নিজে কানেক্ট করবে।

## Folder Structure

```
topupbuzz-clone/
├── index.html          → Home Page
├── login.html          → Login Page
├── contact.html        → Contact Us
├── topup.html          → All Topup Packages
├── about.html          → About Us
├── terms.html          → Terms & Conditions
├── privacy.html        → Privacy Policy
├── refund.html         → Refund Policy
├── delete-account.html → Delete Account Policy
├── css/
│   └── style.css       → Shared Custom CSS
├── js/                 → (তুমি নিজের JS রাখতে পারো)
└── images/             → (প্রোডাক্ট ছবি রাখো)
```

## Tech Stack

- Bootstrap 5.3
- Font Awesome 6
- Noto Sans Bengali (Google Fonts)
- Pure HTML + Custom CSS

## Backend Integration Points

### 1. Login (`login.html`)
```js
// Form submit → POST /api/login
// Google button → Google OAuth
```

### 2. Product Cards (`topup.html` + `index.html`)
```js
// data-product attribute থেকে product ID নিয়ে
// order modal খোলো অথবা /order/:id এ রিডাইরেক্ট করো
```

### 3. Recent Orders
```js
// Live orders API থেকে fetch করে render করো
// fetch('/api/recent-orders')
```

## How to Run

Simply open `index.html` in browser, or use any static server:

```bash
npx serve .
# or
python -m http.server 3000
```

## Customization

- Product images: `images/` ফোল্ডারে রেখে `<img>` ট্যাগ বসাও
- Colors: `css/style.css` এর `:root` ভ্যারিয়েবল চেঞ্জ করো
- Telegram links: সব পেজে আসল লিংক আপডেট করো
