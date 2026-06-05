# غلاية SMURFETT الذكية - Landing Page

A high-converting, mobile-optimized single-product landing page for the Smart SMURFETT Kettle built with Next.js, TypeScript, Tailwind CSS, and Supabase.

## 🎯 Features

- ✅ **Mobile-First Design**: 100% responsive on all devices
- ✅ **Product Carousel**: Smooth swiping with pagination dots
- ✅ **Features Grid**: 6 feature cards with icons and descriptions
- ✅ **Pricing Section**: Clear pricing with shipping and total
- ✅ **Order Form**: Full form with Supabase integration
- ✅ **Geographic Filtering**: Excludes logistics-restricted areas
- ✅ **FAQ Accordion**: Collapsible frequently asked questions
- ✅ **Thank You Page**: Order confirmation page
- ✅ **Trust Badges**: Security and warranty badges
- ✅ **Facebook Pixel**: Conversion tracking

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/infotjarax-cloud/nextjs-boilerplate.git
cd nextjs-boilerplate
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env.local` file with Supabase credentials:
```bash
VITE_SUPABASE_URL=https://hgduniieilcqyoufpvbv.supabase.co
VITE_SUPABASE_ANON_KEY=sb_publishable_CrTyC_N8kkIf00Lc3dT-EQ_GnCCn9WK
```

4. Run the development server:
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 📁 Project Structure

```
src/
├── app/
│   ├── page.tsx           # Main landing page
│   ├── thank-you/page.tsx # Order confirmation page
│   ├── layout.tsx         # Root layout with RTL support
│   └── globals.css        # Global styles
├── components/
│   ├── Header.tsx         # Header banner
│   ├── GiftCard.tsx       # Gift promotion card
│   ├── ProductCarousel.tsx # Product image carousel
│   ├── ProductHero.tsx    # Product title and badges
│   ├── FeaturesCard.tsx   # Features grid
│   ├── PricingCard.tsx    # Pricing display
│   ├── TrustBadges.tsx    # Trust badges row
│   ├── OrderForm.tsx      # Order form with validation
│   ├── FAQAccordion.tsx   # FAQ section
│   └── CTAButton.tsx      # Sticky CTA button
├── lib/
│   └── supabase.ts        # Supabase client
└── data/
    └── governorates.ts    # Governorate data with filtering
```

## 🛠️ Technologies Used

- **Next.js 16**: React framework
- **TypeScript**: Type safety
- **Tailwind CSS 4**: Utility-first CSS
- **Supabase**: Backend & database
- **React Hooks**: State management

## 📱 Mobile Optimization

- Responsive design with mobile-first approach
- Touch-friendly interface for swiping
- Optimized images and lazy loading
- Sticky CTA button for better conversions

## 🌍 Governorate Filtering

The form excludes the following regions:

- **محافظات الصعيد** (Upper Egypt): Luxor, Aswan, Sohag, Qena, Beni Suef, Fayoum, Minya, New Valley
- **البحر الأحمر** (Red Sea): Red Sea, Hurghada
- **جنوب سيناء** (South Sinai): South Sinai, Sharm El-Sheikh
- **مطروح** (Matrouh): Matrouh, Marsa Matrouh

## 💾 Database Schema

Create an `orders` table in Supabase with the following columns:

```sql
CREATE TABLE orders (
  id BIGINT PRIMARY KEY GENERATED ALWAYS AS IDENTITY,
  full_name TEXT NOT NULL,
  phone TEXT NOT NULL,
  governorate TEXT NOT NULL,
  address TEXT NOT NULL,
  notes TEXT,
  product_name TEXT NOT NULL,
  price INTEGER NOT NULL,
  shipping_cost INTEGER NOT NULL,
  total INTEGER NOT NULL,
  status TEXT DEFAULT 'pending',
  created_at TIMESTAMP DEFAULT now()
);
```

## 📊 Conversion Tracking

- Facebook Pixel integrated on thank you page
- Ad account: 4108770199438034
- Pixel ID: 1181131837556431

## 🔒 Security

- Environment variables for sensitive data
- Input validation on client and server
- Phone number validation for Egyptian format
- Supabase authentication with public key

## 📈 Performance

- Optimized for mobile browsers
- Lazy loading for images
- Minimal JavaScript for faster load times
- CSS animations for smooth UX

## 🎨 Branding

- **Primary Color**: Orange (#FF6B00)
- **Secondary Color**: Green (#00C853)
- **Font**: Cairo (Arabic-friendly)
- **Direction**: RTL (Right-to-Left) for Arabic

## 📞 Support

For issues or questions, contact: support@tigarax.store

## 📄 License

This project is private and owned by Tigarax Store.

---

**Made with ❤️ for Egyptian market**
