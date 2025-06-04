# Next.js E-Commerce Platform

A modern, full-stack e-commerce application built with Next.js, featuring user authentication, product management, shopping cart, and secure checkout.

## 🚀 Features

- **User Authentication**: Registration, login, password reset, email verification
- **Product Catalog**: Browse, search, filter, and view detailed product information
- **Shopping Cart**: Add/remove items, quantity management, persistent cart
- **Secure Checkout**: Multiple payment methods, order processing
- **User Dashboard**: Order history, profile management, wishlist
- **Admin Panel**: Product management, order management, analytics
- **Responsive Design**: Mobile-first approach with modern UI/UX
- **SEO Optimized**: Server-side rendering and meta tag management

## 🗺️ Routing Structure

### Public Routes

- **Landing Page** - `/`
- **Product Catalog** - `/products`
- **Product Details** - `/products/[slug]`
- **Product Search** - `/products/search?q=[query]`
- **Product Categories** - `/categories/[category]`
- **About Us** - `/about`
- **Contact** - `/contact`
- **Privacy Policy** - `/privacy`
- **Terms of Service** - `/terms`

### Authentication Routes

- **Login** - `/auth/login`
- **Register** - `/auth/register`
- **Forgot Password** - `/auth/forgot-password`
- **Reset Password** - `/auth/reset-password`
- **Email Verification** - `/auth/email-verify`
- **Two-Factor Auth** - `/auth/2fa`

### User Dashboard (Protected Routes)

- **Dashboard Home** - `/dashboard`
- **Profile Settings** - `/dashboard/profile`
- **Order History** - `/dashboard/orders`
- **Order Details** - `/dashboard/orders/[orderId]`
- **Wishlist** - `/dashboard/wishlist`
- **Addresses** - `/dashboard/addresses`
- **Payment Methods** - `/dashboard/payment-methods`
- **Account Settings** - `/dashboard/settings`

### Shopping & Checkout

- **Shopping Cart** - `/cart`
- **Checkout** - `/checkout`
- **Order Confirmation** - `/checkout/success/[orderId]`
- **Payment Failed** - `/checkout/failed`

### Admin Panel (Protected Routes)

- **Admin Dashboard** - `/admin`
- **Product Management** - `/admin/products`
- **Add Product** - `/admin/products/new`
- **Edit Product** - `/admin/products/[id]/edit`
- **Order Management** - `/admin/orders`
- **Order Details** - `/admin/orders/[orderId]`
- **User Management** - `/admin/users`
- **Category Management** - `/admin/categories`
- **Analytics** - `/admin/analytics`
- **Settings** - `/admin/settings`

### API Routes

- **Authentication** - `/api/auth/*`
- **Products** - `/api/products/*`
- **Cart** - `/api/cart/*`
- **Orders** - `/api/orders/*`
- **Users** - `/api/users/*`
- **Payment** - `/api/payment/*`
- **Search** - `/api/search`
- **Categories** - `/api/categories/*`
- **Reviews** - `/api/reviews/*`

## 🛠️ Tech Stack

- **Frontend**: Next.js 14, React 18, TypeScript
- **Styling**: Tailwind CSS, Shadcn/ui
- **Authentication**: NextAuth.js
- **Database**: PostgreSQL with Prisma ORM
- **Payment**: Stripe
- **Image Storage**: Cloudinary
- **Email**: Resend
- **Deployment**: Vercel

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/next-ecommerce.git
cd next-ecommerce
```

2. Install dependencies:

```bash
npm install
```

3. Set up environment variables:

```bash
cp .env.example .env.local
```

4. Configure your `.env.local` file with:

```env
DATABASE_URL=""
NEXTAUTH_SECRET=""
NEXTAUTH_URL=""
STRIPE_SECRET_KEY=""
STRIPE_PUBLISHABLE_KEY=""
CLOUDINARY_CLOUD_NAME=""
CLOUDINARY_API_KEY=""
CLOUDINARY_API_SECRET=""
RESEND_API_KEY=""
```

5. Run database migrations:

```bash
npx prisma generate
npx prisma db push
```

6. Start the development server:

```bash
npm run dev
```

## 🚀 Deployment

This project is optimized for deployment on Vercel:

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Configure environment variables in Vercel dashboard
4. Deploy!

## 📱 MVP Features Checklist

### Core E-commerce Features

- [ ] Product catalog with search and filtering
- [ ] Shopping cart functionality
- [ ] User authentication and registration
- [ ] Secure checkout process
- [ ] Order management
- [ ] Payment integration (Stripe)
- [ ] Email notifications
- [ ] Responsive design

### User Experience

- [ ] Product reviews and ratings
- [ ] Wishlist functionality
- [ ] Order tracking
- [ ] Guest checkout option
- [ ] Mobile-optimized interface
- [ ] Fast loading times
- [ ] SEO optimization

### Admin Features

- [ ] Product management (CRUD)
- [ ] Order management
- [ ] User management
- [ ] Basic analytics
- [ ] Inventory tracking

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support, email support@yourecommerce.com or join our Discord community.
