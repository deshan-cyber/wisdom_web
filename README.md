✦ Spiritual Growth & Course
Platform
Complete Fullstack Website Blueprint
Share your spiritual wisdom · Sell courses · Build community
Property Value
Document type Full-Stack Development Blueprint
Purpose Build a spiritual knowledge + course-selling website
Tech stack React · Node.js · MongoDB · Stripe · AWS S3
Audience First-time web developer (you!)
Covers Architecture · Pages · Backend · Payments · Deployment
■ How to use this
document
Read it top-to-bottom the first time to understand the full picture.
Then use each chapter as a step-by-step checklist while you build.
Every code snippet is ready to copy. Every tool recommendation is
free-tier friendly for beginners.
Spiritual Growth & Course Platform — Full Blueprint | Page 2
Table of Contents
Chapter 1 — What This Website Does
– Core purpose
– Who it serves
– What you will earn
Chapter 2 — Website Structure & All Pages
– Homepage
– Blog / Wisdom Articles
– Podcast page
– About page
– Courses catalogue
– Single course page
– User dashboard
– Login / Register
– Checkout & payment
– Admin panel
Chapter 3 — Technology Stack — Explained Simply
– Frontend (what visitors see)
– Backend (your server)
– Database
– File storage
– Email
– Payments
Chapter 4 — Project Folder Structure
– Frontend layout
– Backend layout
– Naming conventions
Chapter 5 — Frontend Build Guide
– Setting up React
– Routing
– Key components
– Styling approach
– State management
Chapter 6 — Backend Build Guide
– Setting up Node/Express
– Authentication (JWT)
– Course CRUD APIs
– Blog APIs
– File upload APIs
Chapter 7 — Database Design (MongoDB)
– User schema
– Course schema
– Blog post schema
– Purchase/enrolment schema
Spiritual Growth & Course Platform — Full Blueprint | Page 3
– Comments schema
Chapter 8 — Course & Content Delivery
– Video hosting options
– PDF delivery
– Locking paid content
– Progress tracking
Chapter 9 — Payment Integration (Stripe)
– How Stripe works
– One-time purchase
– Subscription plan
– Webhook setup
– Refund logic
Chapter 10 — Authentication & Security
– JWT flow
– Passwords
– Protected routes
– Rate limiting
– HTTPS
Chapter 11 — Admin Panel
– Dashboard metrics
– Manage courses
– Manage users
– Blog management
– Revenue view
Chapter 12 — Email Automation
– Welcome email
– Purchase confirmation
– Course drip emails
– Newsletter
Chapter 13 — SEO & Performance
– Meta tags
– Sitemap
– Image optimisation
– Page speed tips
Chapter 14 — Deployment Step-by-Step
– Frontend on Vercel
– Backend on Render
– Database on MongoDB Atlas
– Domain & SSL
Chapter 15 — Costs & Free Tier Summary
– What is free
– What costs money
– Realistic monthly budget
Chapter 16 — Launch Checklist
– Pre-launch
Spiritual Growth & Course Platform — Full Blueprint | Page 4
– Launch day
– First 30 days
Chapter 17 — Recommended Learning Resources
Spiritual Growth & Course Platform — Full Blueprint | Page 5
Chapter 1
What This Website Does & Why It Matters
Your Mission Statement
You have walked through real struggles — rejection, self-doubt, fear — and you came out with
hard-won spiritual wisdom. This website is your platform to share that journey and help others do the
same. It is not just a blog or a course shop. It is a living, breathing community built around
transformation.
What the site does for visitors:
• Reads your free articles on confidence, handling rejection, inner peace, purpose.
• Watches or listens to your free content (videos / podcast).
• Discovers paid courses that go deeper with exercises, workbooks, and personal guidance.
• Creates an account, tracks their progress, and joins a community.
• Gets email inspiration from you on a regular schedule.
What the site does for YOU:
Revenue / Value stream How it works
Free articles & content Builds trust, attracts Google traffic, grows your audience
Paid courses (one-time) e.g. $49 course — you keep ~97% after Stripe fees
Paid courses (monthly subscription) Recurring income, e.g. $19/mo membership
Email list Direct access to your audience — no algorithm needed
Admin dashboard See revenue, users, popular content in one place
★ Inspiring example
Many solo creators earn $3,000–$20,000/month from a simple course website
with fewer than 2,000 email subscribers. Your authentic spiritual story is
the product.
Spiritual Growth & Course Platform — Full Blueprint | Page 6
Chapter 2
Every Page Your Website Needs
Homepage /
Hero section with your photo + tagline. 3 featured articles. 'Start here' journey path. Testimonials. Email
opt-in. Featured course banner.
• Hero headline + sub-headline + CTA button
• 3-card free article preview
• Journey section: 'From struggle → insight → transformation'
• 2-3 student testimonials (photo + quote)
• Email sign-up box with a free gift (e.g. PDF guide)
• 1 featured course card
Blog / Wisdom /blog
All your free articles. Filter by topic (confidence, rejection, purpose, etc.).
• Article grid with thumbnail, title, 2-line excerpt
• Category filter tabs
• Search bar
• Pagination or infinite scroll
Single Article /blog/:slug
Full article with rich formatting.
• Author bio box
• Table of contents
• Related articles
• Email opt-in within article
• Share buttons
Courses /courses
Catalogue of all your paid (and free preview) courses.
• Course cards: title, image, short desc, price, star rating
• Filter by category / price
Spiritual Growth & Course Platform — Full Blueprint | Page 7
• Bestseller / New badge
Single Course /courses/:slug
Full sales page for one course.
• Course title + tagline
• Promo video (free preview)
• What you'll learn (bullet list)
• Full curriculum accordion
• Instructor bio
• Student reviews
• Sticky 'Enrol now' sidebar with price + CTA
User Dashboard /dashboard
After login — shows their enrolled courses and progress.
• My courses list
• Continue watching button
• Progress bar per course
• Certificates earned
Login / Register /login /register
Simple clean forms.
• Email + password
• Google OAuth (optional)
• Forgot password flow
Checkout /checkout
Stripe-powered payment page.
• Order summary
• Stripe card element
• Apply coupon code
• Secure badges
About /about
Spiritual Growth & Course Platform — Full Blueprint | Page 8
Your personal story — the spiritual struggle and the breakthrough.
• Your photo
• Your story (long-form)
• Your values / philosophy
• Press / media mentions
Contact /contact
Simple form + social links.
• Name, email, message
• Social media links
• Response time notice
Admin /admin/*
Hidden from public. Only you can access.
• Dashboard: revenue chart, new users, course sales
• Courses: create / edit / delete
• Blog posts: draft / publish
• Users: list, ban, refund
• Coupons: create discount codes
Spiritual Growth & Course Platform — Full Blueprint | Page 9
Chapter 3
Technology Stack — Explained Simply
Think of your website like a restaurant. The frontend is the dining room — what customers see and
touch. The backend is the kitchen — where the work happens. The database is the pantry — where
everything is stored.
Layer Technology Why this choice
Frontend (UI) React.js Most popular, huge job market, reusable components
Styling Tailwind CSS Write styles fast without leaving your HTML
Routing React Router v6 Navigate between pages without page reloads
Backend Node.js + Express JavaScript on the server — same language
front+back
Database MongoDB Atlas Flexible document store, free tier, cloud-hosted
Auth JWT tokens Secure stateless authentication, easy to implement
File/Video AWS S3 or
Cloudinary
Store course videos, PDFs, images cheaply
Payments Stripe Industry standard, great docs, 2.9% + 30¢ per charge
Email Resend / SendGrid Transactional + marketing emails, generous free tier
Deployment FE Vercel Free, instant deploys, great for React
Deployment BE Render.com Free tier for Node APIs, easy setup
✓ Beginner tip
You do NOT need to learn all of this at once. Start with React + Node +
MongoDB. Add Stripe when your first page is working. Add email last. Build
in layers.
Spiritual Growth & Course Platform — Full Blueprint | Page 10
Chapter 4
Project Folder Structure
Frontend (React app)
spiritual-platform/
client/
public/
index.html
src/
components/ ← reusable UI pieces (Button, Card, Navbar)
pages/ ← one file per route (Home.jsx, Courses.jsx …)
context/ ← global state (AuthContext, CartContext)
hooks/ ← custom React hooks (useCourses, useAuth)
services/ ← API call functions (courseService.js)
utils/ ← helper functions
styles/ ← global CSS or Tailwind config
App.jsx ← root component + router
main.jsx ← entry point
package.json
tailwind.config.js
vite.config.js
Backend (Node/Express API)
Spiritual Growth & Course Platform — Full Blueprint | Page 11
server/
config/
db.js ← MongoDB connection
cloudinary.js ← file upload config
controllers/ ← business logic (authController, courseController)
middleware/
auth.js ← JWT verify middleware
isAdmin.js ← admin-only middleware
upload.js ← multer file handler
models/ ← MongoDB schemas (User, Course, Post …)
routes/ ← Express routers (authRoutes, courseRoutes …)
utils/
sendEmail.js ← email helper
generateToken.js ← JWT helper
server.js ← main entry, middleware setup
.env ← secrets (NEVER commit this)
package.json
! Important
Never commit your .env file to GitHub. Add it to .gitignore immediately.
It contains your database password, Stripe keys, and JWT secret.
Spiritual Growth & Course Platform — Full Blueprint | Page 12
Chapter 5
Frontend Build Guide
1. Create your React project
# In your terminal:
npm create vite@latest client -- --template react
cd client
npm install
# Install key libraries:
npm install react-router-dom axios tailwindcss @headlessui/react
npm install react-query react-hook-form @stripe/react-stripe-js
npm install react-player react-hot-toast lucide-react
2. Configure routing (App.jsx)
import { BrowserRouter, Routes, Route } from 'react-router-dom';
import ProtectedRoute from './components/ProtectedRoute';
function App() {
return (
} />
} />
} />
} />
} />
} />
} />
} />
} />
} />
);
}
Spiritual Growth & Course Platform — Full Blueprint | Page 13
3. Auth Context (global login state)
// src/context/AuthContext.jsx
import { createContext, useContext, useState, useEffect } from 'react';
const AuthContext = createContext();
export function AuthProvider({ children }) {
const [user, setUser] = useState(
JSON.parse(localStorage.getItem('user')) || null
);
const login = (userData) => {
setUser(userData);
localStorage.setItem('user', JSON.stringify(userData));
};
const logout = () => {
setUser(null);
localStorage.removeItem('user');
};
return (
{children}
);
}
export const useAuth = () => useContext(AuthContext);
4. Key reusable components to build
Component file What it does
Navbar.jsx Logo, nav links, login/logout button, mobile hamburger
Footer.jsx Links, social icons, copyright
CourseCard.jsx Thumbnail, title, price, star rating, CTA button
BlogCard.jsx Category tag, title, excerpt, read time
ProtectedRoute.jsx Redirects to /login if not authenticated
AdminRoute.jsx Redirects if not admin
Spiritual Growth & Course Platform — Full Blueprint | Page 14
VideoPlayer.jsx Wraps react-player, locked if not enrolled
StarRating.jsx Display + submit star ratings
ProgressBar.jsx Shows % complete in dashboard
Modal.jsx Reusable popup for confirmations
Spiritual Growth & Course Platform — Full Blueprint | Page 15
Chapter 6
Backend Build Guide (Node.js + Express)
1. Initial server setup
# Create server folder
mkdir server && cd server
npm init -y
npm install express mongoose dotenv bcryptjs jsonwebtoken
npm install multer cloudinary cors morgan helmet express-rate-limit
npm install stripe nodemailer
npm install --save-dev nodemon
2. server.js — main entry point
Spiritual Growth & Course Platform — Full Blueprint | Page 16
require('dotenv').config();
const express = require('express');
const cors = require('cors');
const helmet = require('helmet');
const rateLimit = require('express-rate-limit');
const connectDB = require('./config/db');
const app = express();
connectDB();
app.use(helmet());
app.use(cors({ origin: process.env.CLIENT_URL, credentials: true }));
app.use(express.json());
app.use(rateLimit({ windowMs: 15*60*1000, max: 100 }));
// Routes
app.use('/api/auth', require('./routes/authRoutes'));
app.use('/api/courses', require('./routes/courseRoutes'));
app.use('/api/blog', require('./routes/blogRoutes'));
app.use('/api/payment', require('./routes/paymentRoutes'));
app.use('/api/admin', require('./routes/adminRoutes'));
app.listen(process.env.PORT || 5000,
() => console.log('Server running on port 5000'));
3. Auth controller — register & login
Spiritual Growth & Course Platform — Full Blueprint | Page 17
// controllers/authController.js
const bcrypt = require('bcryptjs');
const jwt = require('jsonwebtoken');
const User = require('../models/User');
exports.register = async (req, res) => {
try {
const { name, email, password } = req.body;
const exists = await User.findOne({ email });
if (exists) return res.status(400).json({ msg: 'Email in use' });
const hash = await bcrypt.hash(password, 12);
const user = await User.create({ name, email, password: hash });
const token = jwt.sign(
{ id: user._id, isAdmin: user.isAdmin },
process.env.JWT_SECRET,
{ expiresIn: '7d' }
);
res.status(201).json({ token, user: { id: user._id, name, email } });
} catch(err) { res.status(500).json({ msg: err.message }); }
};
4. Auth middleware
// middleware/auth.js
const jwt = require('jsonwebtoken');
module.exports = (req, res, next) => {
const token = req.headers.authorization?.split(' ')[1];
if (!token) return res.status(401).json({ msg: 'No token' });
try {
req.user = jwt.verify(token, process.env.JWT_SECRET);
next();
} catch { res.status(401).json({ msg: 'Token invalid' }); }
};
5. API routes overview
Spiritual Growth & Course Platform — Full Blueprint | Page 18
Endpoint What it does
POST /api/auth/register Create new user account
POST /api/auth/login Return JWT token
GET /api/courses List all published courses
GET /api/courses/:slug Single course details
POST /api/courses (admin) Create a course
PUT /api/courses/:id (admin) Edit a course
GET /api/blog List published articles
GET /api/blog/:slug Single article
POST /api/blog (admin) Create article
POST /api/payment/checkout Create Stripe payment intent
POST /api/payment/webhook Stripe webhook → grant access
GET /api/admin/stats (admin) Revenue, user counts, top courses
Spiritual Growth & Course Platform — Full Blueprint | Page 19
Chapter 7
Database Design — MongoDB Schemas
User schema
• name: String (required)
• email: String (required, unique, lowercase)
• password: String (hashed, min 6 chars)
• isAdmin: Boolean (default: false)
• enrolledCourses: [{ courseId, enrolledAt, progress: 0–100 }]
• createdAt: Date (auto)
Course schema
• title: String (required)
• slug: String (unique, auto-generated from title)
• description: String
• shortDesc: String (for cards)
• price: Number
• isSubscription: Boolean
• thumbnail: String (URL)
• previewVideo: String (URL)
• curriculum: [{ sectionTitle, lessons: [{ title, videoUrl, duration, isFree }] }]
• instructor: ObjectId (ref User)
• category: String
• tags: [String]
• ratings: [{ user, score, review }]
• isPublished: Boolean
Blog post schema
• title: String
• slug: String (unique)
• content: String (rich HTML or Markdown)
• excerpt: String
• coverImage: String (URL)
Spiritual Growth & Course Platform — Full Blueprint | Page 20
• author: ObjectId (ref User)
• category: String
• tags: [String]
• isPublished: Boolean
• publishedAt: Date
Purchase schema
• user: ObjectId (ref User)
• course: ObjectId (ref Course)
• stripePaymentId: String
• amount: Number
• currency: String
• status: String (pending | completed | refunded)
• createdAt: Date
MongoDB connection (config/db.js)
const mongoose = require('mongoose');
const connectDB = async () => {
try {
await mongoose.connect(process.env.MONGO_URI);
console.log('MongoDB connected');
} catch(err) {
console.error(err.message);
process.exit(1);
}
};
module.exports = connectDB;
Spiritual Growth & Course Platform — Full Blueprint | Page 21
Chapter 8
Course & Content Delivery
Video hosting options
Option Cost Notes
Vimeo (Recommended) $12–20/mo Private links, no ads, clean player
Cloudinary Free–$89/mo Easy to use, also handles images
AWS S3 + CloudFront ~$0.02/GB Cheapest at scale, needs more setup
YouTube (Unlisted) Free Easy but YouTube branding, less professional
Bunny.net CDN $0.01/GB Cheapest video CDN, great for beginners
Locking paid content — the pattern
// Backend — check enrollment before serving video URL
router.get('/courses/:id/lesson/:lessonId', auth, async (req, res) => {
const user = await User.findById(req.user.id);
const enrolled = user.enrolledCourses.some(
e => e.courseId.toString() === req.params.id
);
if (!enrolled) return res.status(403).json({ msg: 'Purchase required' });
const course = await Course.findById(req.params.id);
const lesson = course.curriculum
.flatMap(s => s.lessons)
.find(l => l._id.toString() === req.params.lessonId);
res.json({ videoUrl: lesson.videoUrl }); // URL never exposed publicly
});
Progress tracking
Spiritual Growth & Course Platform — Full Blueprint | Page 22
// Mark lesson complete
router.post('/courses/:id/lesson/:lessonId/complete', auth, async (req, res) => {
await User.updateOne(
{ _id: req.user.id, 'enrolledCourses.courseId': req.params.id },
{ $addToSet: { 'enrolledCourses.$.completedLessons': req.params.lessonId } }
);
res.json({ msg: 'Progress saved' });
});
Spiritual Growth & Course Platform — Full Blueprint | Page 23
Chapter 9
Stripe Payment Integration
How Stripe works in plain English
1. User clicks 'Enrol now' → your frontend asks your backend for a Payment Intent (a unique payment
session). 2. Stripe's secure card form collects the card details — you never touch card numbers. 3.
Stripe processes the payment and sends a webhook (a ping) to your server. 4. Your server grants the
user access to the course.
Backend — create payment intent
const stripe = require('stripe')(process.env.STRIPE_SECRET_KEY);
router.post('/checkout', auth, async (req, res) => {
const { courseId } = req.body;
const course = await Course.findById(courseId);
const paymentIntent = await stripe.paymentIntents.create({
amount: course.price * 100, // Stripe uses cents
currency: 'usd',
metadata: { courseId, userId: req.user.id },
});
res.json({ clientSecret: paymentIntent.client_secret });
});
Frontend — payment form with Stripe Elements
Spiritual Growth & Course Platform — Full Blueprint | Page 24
import { loadStripe } from '@stripe/stripe-js';
import { Elements, CardElement, useStripe, useElements } from
'@stripe/react-stripe-js';
const stripePromise = loadStripe(process.env.REACT_APP_STRIPE_PUBLIC_KEY);
function CheckoutForm({ courseId }) {
const stripe = useStripe();
const elements = useElements();
const handleSubmit = async (e) => {
e.preventDefault();
const { data } = await axios.post('/api/payment/checkout', { courseId });
const result = await stripe.confirmCardPayment(data.clientSecret, {
payment_method: { card: elements.getElement(CardElement) }
});
if (result.paymentIntent?.status === 'succeeded') {
navigate('/dashboard');
}
};
return Pay;
}
Webhook — grant access after payment
Spiritual Growth & Course Platform — Full Blueprint | Page 25
router.post('/webhook', express.raw({type:'application/json'}), async (req, res) =>
{
const sig = req.headers['stripe-signature'];
const event = stripe.webhooks.constructEvent(
req.body, sig, process.env.STRIPE_WEBHOOK_SECRET
);
if (event.type === 'payment_intent.succeeded') {
const { courseId, userId } = event.data.object.metadata;
await User.findByIdAndUpdate(userId, {
$addToSet: { enrolledCourses: { courseId, enrolledAt: new Date() } }
});
await Purchase.create({ user: userId, course: courseId,
stripePaymentId: event.data.object.id,
amount: event.data.object.amount / 100,
status: 'completed' });
}
res.json({ received: true });
});
Spiritual Growth & Course Platform — Full Blueprint | Page 26
Chapter 10
Authentication & Security
Security checklist for beginners
Passwords — Always hash with bcrypt (saltRounds: 12). Never store plain text.
JWT secrets — Use a long random string (32+ chars). Rotate it if compromised.
HTTPS — Vercel and Render give you free SSL. Always use it in production.
CORS — Only allow your frontend domain, not '*' in production.
Rate limiting — Limit /api/auth routes to ~10 requests/minute to prevent brute force.
Helmet.js — Adds security headers automatically. Already in the server setup.
Input validation — Use express-validator to check all user inputs server-side.
.env — Never commit secrets. Use environment variable panels on Render/Vercel.
Admin routes — Double-check every admin route has both auth + isAdmin middleware.
Stripe webhooks — Verify webhook signatures — anyone can fake a POST request otherwise.
.env file template
# server/.env
PORT=5000
MONGO_URI=mongodb+srv://youruser:password@cluster.mongodb.net/spiritual
JWT_SECRET=put_a_very_long_random_string_here_32_chars_min
CLIENT_URL=http://localhost:3000
STRIPE_SECRET_KEY=sk_test_...
STRIPE_WEBHOOK_SECRET=whsec_...
CLOUDINARY_CLOUD_NAME=your_cloud
CLOUDINARY_API_KEY=123456
CLOUDINARY_API_SECRET=abcdef
EMAIL_FROM=you@yourdomain.com
RESEND_API_KEY=re_...
Spiritual Growth & Course Platform — Full Blueprint | Page 27
Chapter 11
Admin Panel
Your admin panel lives at /admin and is only accessible when isAdmin is true. Build it as a separate
mini-app inside your React project.
Route Page Key features
/admin Dashboard Revenue this week/month, total users, new signups
chart, top 3 courses
/admin/courses Courses list Table of all courses with edit/delete. Toggle
published.
/admin/courses/new Create course Form: title, description, price, upload thumbnail, add
curriculum sections & lessons
/admin/blog Blog list All posts, draft/published status, quick edit
/admin/blog/new Write post Rich text editor (use react-quill or TipTap)
/admin/users Users list Search by email, see enrollments, ban/unban
/admin/revenue Revenue Table of all purchases. Filter by date. Export CSV.
/admin/coupons Coupons Create discount codes (% or fixed), set expiry &
usage limit
Spiritual Growth & Course Platform — Full Blueprint | Page 28
Chapter 12
Email Automation
Why email matters more than social media
Your email list is the one audience you own. Social platforms can change their algorithm tomorrow and
your reach drops to zero. A 1,000-person email list is worth more than 10,000 social followers for
selling courses.
Email flows to build
Email Purpose & content
Welcome email Sent immediately on sign-up. Introduce yourself, link to 'start
here' article, set expectations.
Free gift delivery If they signed up for a free PDF/guide, deliver it here. High
open rate.
Purchase confirmation Sent after Stripe payment. Order summary + link to their
dashboard.
Course access Email with login link and direct link to first lesson.
Day 3 check-in Did they start the course? If not, a gentle nudge.
Weekly wisdom Short email every week. 1 insight from you. Builds trust.
New course launch Announce to your list. Early-bird price for 48 hours.
Sending emails with Resend (simplest option)
Spiritual Growth & Course Platform — Full Blueprint | Page 29
// utils/sendEmail.js
const { Resend } = require('resend');
const resend = new Resend(process.env.RESEND_API_KEY);
async function sendEmail({ to, subject, html }) {
await resend.emails.send({
from: 'You ',
to,
subject,
html,
});
}
module.exports = sendEmail;
// Usage after successful purchase:
await sendEmail({
to: user.email,
subject: 'Your course access is ready!',
html: `Welcome, ${user.name}!
Click here to start: Go to dashboard`
});
Spiritual Growth & Course Platform — Full Blueprint | Page 30
Chapter 13
SEO & Performance
Dynamic meta tags per page (React Helmet)
npm install react-helmet-async
// In each page component:
import { Helmet } from 'react-helmet-async';
function ArticlePage({ post }) {
return (
<>
{post.title} | YourSiteName
{/* page content */}
);
}
SEO quick wins
• Use descriptive slugs: /blog/how-to-build-confidence-after-rejection (not /blog/post-1)
• Add alt text to every image: alt='description of image' on every img tag
• Write 1,500+ word articles — Google favours depth
• Submit your sitemap to Google Search Console (free)
• Load speed: compress images with TinyPNG before uploading
• Use Lighthouse in Chrome DevTools to audit performance
• Internal links: link from blog articles to your course pages
• Get backlinks: guest post on spiritual/self-help blogs in your first 3 months
★ Highest value SEO action
Write one 2,000-word article per week for 3 months targeting phrases like
'how to overcome rejection spiritually', 'building confidence through
faith', etc. This alone can bring hundreds of free visitors per month.
Spiritual Growth & Course Platform — Full Blueprint | Page 31
Chapter 14
Deployment — Step by Step
Step 1: Deploy database to MongoDB Atlas
• Go to mongodb.com/atlas → create free account
• Create a free M0 cluster (512MB free forever)
• Create a database user with username + password
• Whitelist all IPs: 0.0.0.0/0 (you can restrict later)
• Copy the connection string → save as MONGO_URI in your .env
Step 2: Deploy backend to Render.com
• Push your server/ folder to a GitHub repo
• Go to render.com → New → Web Service
• Connect your GitHub repo
• Build command: npm install | Start command: node server.js
• Add all .env variables in the Environment tab
• Deploy! Render gives you a free URL like https://your-api.onrender.com
• Copy this URL — you'll need it for the frontend
Step 3: Deploy frontend to Vercel
• Push your client/ folder to GitHub (can be same repo, different folder)
• Go to vercel.com → New Project → Import from GitHub
• Set root directory to client/
• Add env variable: REACT_APP_API_URL = https://your-api.onrender.com
• Deploy! Vercel gives you a free .vercel.app domain
Step 4: Add your custom domain
• Buy a domain on Namecheap or Google Domains (~$12/yr)
• In Vercel settings → Domains → add your domain
• Update nameservers or add DNS records as Vercel instructs
• SSL certificate is automatic (free via Let's Encrypt)
• Update CORS in your backend: CLIENT_URL=https://yourdomain.com
Spiritual Growth & Course Platform — Full Blueprint | Page 32
Step 5: Set up Stripe webhook for production
• In Stripe dashboard → Developers → Webhooks → Add endpoint
• URL: https://your-api.onrender.com/api/payment/webhook
• Events to listen for: payment_intent.succeeded
• Copy the webhook secret → add as STRIPE_WEBHOOK_SECRET in Render
Spiritual Growth & Course Platform — Full Blueprint | Page 33
Chapter 15
Costs & Free Tier Summary
What you can start with for free
Service Category Free tier
MongoDB Atlas M0 Database 512MB, 1 cluster — enough for thousands of users
Render.com (free) Backend hosting 750 hrs/mo, sleeps after 15 min of inactivity
Vercel (free) Frontend hosting Unlimited deploys, custom domain, SSL
Stripe Payments No monthly fee — just 2.9% + 30¢ per transaction
Resend Email 3,000 emails/month free
Cloudinary Images/video 25GB storage, 25GB bandwidth/month free
GitHub Code storage Unlimited public/private repos
Realistic monthly costs as you grow
Stage Monthly cost Notes
Starting out (0–50 students) $0 – $20/mo Domain ($1/mo) + possibly Vimeo starter
Growing (50–200 students) $30 – $80/mo Render paid ($7), Vimeo Plus ($20), email tool
($10+)
Established (200+ students) $80 – $200/mo Better hosting, CDN, premium tools
Your revenue at 200 students $5,000–$20,000
+
Depends on course price (avg $97)
✓ Bottom line
You can launch this entire platform for under $15/month. With a single $97
course sale your first month, you are already profitable.
Spiritual Growth & Course Platform — Full Blueprint | Page 34
Chapter 16
Launch Checklist
Pre-launch (2 weeks before)
■ Homepage is live with hero, about section, email opt-in
■ At least 3 blog articles published
■ At least 1 complete course ready (all videos, workbook PDF)
■ Stripe test mode payments working end-to-end
■ Switch Stripe to LIVE mode
■ Custom domain pointing to Vercel
■ SSL certificate active (check for padlock in browser)
■ All .env secrets set on Render and Vercel
■ Webhook secret set in Stripe dashboard (production)
■ Test register → purchase → dashboard access flow
■ Mobile responsive check on iPhone and Android
■ 404 page exists
■ Privacy policy and terms of service pages exist
■ Google Analytics or Plausible connected
Launch day
■ Post your story on LinkedIn / Instagram
■ Send email to anyone who signed up during beta
■ Post in relevant Facebook groups / Reddit communities (authentic, not spam)
■ Monitor Render logs for errors in real time
■ Check Stripe dashboard for incoming payments
First 30 days
■ Publish 2 new blog articles per week
■ Send 1 email per week to your list
■ Respond to every single comment and question personally
■ Ask your first 5 students for a testimonial
■ Set up a 'course complete' certificate (use Canva template)
■ Analyse which blog articles get the most traffic (Google Search Console)
■ Plan your second course based on student questions
Spiritual Growth & Course Platform — Full Blueprint | Page 35
Chapter 17
Recommended Learning Resources
Topic Resource
React basics react.dev (official docs) — start with 'Learn React' tutorial
Node + Express expressjs.com + The Odin Project (free, full curriculum)
MongoDB mongodb.com/docs + 'MongoDB University' free courses
Tailwind CSS tailwindcss.com/docs — best CSS framework docs ever
written
Stripe integration stripe.com/docs/payments/quickstart — official tutorial
Full-stack project YouTube: 'MERN Stack Course 2024' by freeCodeCamp
(7hrs, free)
Deployment docs.render.com and vercel.com/docs — both have great
guides
Web security basics OWASP Top 10 (owasp.org) — essential reading
Git & GitHub github.com/git-guides — learn version control first
VS Code setup code.visualstudio.com — install ESLint + Prettier extensions
Suggested learning order (total ~3–4 months to launch)
• Week 1–2: HTML + CSS basics (if needed). Set up VS Code + Git.
• Week 3–4: JavaScript fundamentals. Variables, functions, arrays, async/await.
• Week 5–6: React basics. Components, props, state, hooks.
• Week 7–8: Node.js + Express. Build a basic REST API.
• Week 9–10: MongoDB. Connect to Atlas, write Mongoose schemas.
• Week 11: Authentication with JWT. Build login/register.
• Week 12: Stripe integration. Test payment flow end-to-end.
• Week 13: Build your actual site using this blueprint.
• Week 14: Deploy, test, and LAUNCH.
Spiritual Growth & Course Platform — Full Blueprint | Page 36
You have the most important ingredient — a genuine story and a desire to help others. The
code is just the vehicle. Build it one step at a time. You will figure it out. ✦
