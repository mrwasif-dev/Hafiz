AL-HAFIZ ISLAMIC RESEARCH INSTITUTE — WEBSITE PACKAGE
======================================================

WHAT'S INSIDE
-------------
- index.html      Home
- about.html      About / founder / principles
- services.html   All 11 services in detail
- reviews.html    Public client reviews + "add your review" form
- login.html      Log in
- register.html   Create account
- account.html    Logged-in user's account page
- contact.html    Contact form + WhatsApp/Facebook/TikTok links
- css/style.css   All styling, light & dark mode, animations
- js/main.js      Theme toggle, mobile menu, scroll animations
- js/auth.js      Login/Register/Account logic
- js/reviews.js   Reviews list + submission
- js/chatbot.js   The on-site assistant chatbot

HOW TO USE IT
-------------
Just open index.html in a browser, or upload the whole folder to any
web host (Hostinger, GitHub Pages, Netlify, cPanel, etc.) — no build
step needed, it's plain HTML/CSS/JS.

IMPORTANT — ABOUT LOGIN, REVIEWS & THE CHATBOT
------------------------------------------------
This package is a complete, fully working FRONT END. Because it's a
static site (no server included), the account system and reviews
currently save data in the visitor's own browser (localStorage), not
in a shared MongoDB database — so one visitor's account/reviews won't
be visible to a different visitor on a different device yet. The
chatbot answers from a built-in list of your services rather than a
live AI API.

To make accounts, reviews, and the chatbot fully shared and live for
every visitor (as you asked, with a real MongoDB database and a real
AI API), you need a small backend added on top of this front end:

1. A Node.js + Express server with a MongoDB database (e.g. via
   MongoDB Atlas, free tier available) — with a `users` collection
   and a `reviews` collection.
2. Replace the localStorage calls in js/auth.js and js/reviews.js
   with fetch() calls to that server's API (e.g. POST /api/register,
   POST /api/login, GET/POST /api/reviews).
3. For a true AI chatbot (instead of the built-in FAQ list), connect
   js/chatbot.js to the Anthropic API or another AI provider using
   your own API key on the server side (never expose an API key in
   front-end code).

I'm happy to build that backend next if you'd like — just say so and
tell me where you plan to host it (e.g. a VPS, Render, Railway).

CONTACT DETAILS USED IN THE SITE
---------------------------------
WhatsApp (primary / floating button): 0306-1819635
WhatsApp (support chat number):        0332-0033563
WhatsApp Channel, TikTok and Facebook links are in the footer and
Contact page.
Founder name shown throughout: Hafiz Mahmood
