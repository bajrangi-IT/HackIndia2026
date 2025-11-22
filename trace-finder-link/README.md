# 🔍 FINDHOPE

**Helping reunite missing persons with their families through AI-powered facial recognition and community support.**

[![GitHub](https://img.shields.io/badge/GitHub-bajrangi--IT%2FFINDHOPE-blue?logo=github)](https://github.com/bajrangi-IT/FINDHOPE)
[![License](https://img.shields.io/badge/license-MIT-green.svg)]()
[![React](https://img.shields.io/badge/React-18.3.1-61DAFB?logo=react)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8.3-3178C6?logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.4.19-646CFF?logo=vite)](https://vitejs.dev/)

---

## 📖 Overview

**FINDHOPE** is a comprehensive missing person tracking application that leverages the power of AI and community collaboration to help reunite missing individuals with their families. The platform provides tools for reporting missing persons, uploading CCTV footage for analysis, and maintaining a searchable database of cases.

### 🎯 Key Features

- **📝 Report Missing Persons**: Easily file detailed reports with photos, descriptions, and last known locations
- **👤 Facial Recognition**: AI-powered facial matching using Hugging Face's advanced models
- **📹 CCTV Integration**: Upload and analyze CCTV footage to identify potential matches
- **🗺️ Interactive Map**: Google Maps integration to visualize last known locations and sightings
- **🔍 Search & Filter**: Advanced search capabilities to find specific cases
- **📊 Dashboard**: Comprehensive analytics and case management interface
- **🔒 Secure Authentication**: Powered by Supabase for robust user management
- **📱 Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **🌙 Dark Mode Support**: Easy on the eyes during extended use

---

## 🛠️ Technology Stack

### Frontend
- **React 18.3.1** - Modern UI library
- **TypeScript 5.8.3** - Type-safe JavaScript
- **Vite 5.4.19** - Lightning-fast build tool
- **Tailwind CSS 3.4.17** - Utility-first CSS framework
- **shadcn/ui** - Beautiful, accessible component library
- **Radix UI** - Unstyled, accessible UI primitives

### Backend & Services
- **Supabase** - Backend-as-a-Service (Database, Auth, Storage)
- **Supabase Edge Functions** - Serverless functions for AI processing
- **Hugging Face API** - Facial recognition and image analysis

### Additional Libraries
- **React Router DOM** - Client-side routing
- **TanStack React Query** - Data fetching and caching
- **React Hook Form** - Form management
- **Zod** - Schema validation
- **Recharts** - Data visualization
- **QRCode.react** - QR code generation
- **Google Maps API** - Location services
- **jsPDF & html2canvas** - PDF report generation

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- **Node.js** (v18 or higher) - [Download here](https://nodejs.org/)
- **npm** or **yarn** - Comes with Node.js
- **Git** - [Download here](https://git-scm.com/)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/bajrangi-IT/FINDHOPE.git
   cd FINDHOPE
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory:
   ```env
   VITE_SUPABASE_URL=your_supabase_project_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   VITE_GOOGLE_MAPS_API_KEY=your_google_maps_api_key
   VITE_HUGGINGFACE_API_KEY=your_huggingface_api_key
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   
   Navigate to `http://localhost:5173` (or the port shown in your terminal)

---

## 📦 Build for Production

To create a production-ready build:

```bash
npm run build
```

The optimized files will be in the `dist` folder.

To preview the production build locally:

```bash
npm run preview
```

---

## 🗄️ Supabase Setup

### 1. Create a Supabase Project

1. Go to [Supabase](https://supabase.com/)
2. Create a new project
3. Copy your project URL and anon key to the `.env` file

### 2. Database Schema

The application requires the following tables:
- `missing_persons` - Stores missing person reports
- `cctv_images` - Stores uploaded CCTV images
- `matches` - Stores facial recognition matches
- `profiles` - User profiles

### 3. Edge Functions

Deploy the Supabase Edge Functions located in the `supabase/functions` directory:

```bash
# Install Supabase CLI
npm install -g supabase

# Log in to Supabase
supabase login

# Link your project
supabase link --project-ref your-project-ref

# Deploy functions
supabase functions deploy match-photo
supabase functions deploy process-cctv-image
```

### 4. Storage Buckets

Create the following storage buckets in Supabase:
- `missing-persons-photos`
- `cctv-images`

Enable public access for these buckets if needed.

---

## 🔑 API Keys Setup

### Hugging Face API

1. Create an account at [Hugging Face](https://huggingface.co/)
2. Generate an API token from your [settings](https://huggingface.co/settings/tokens)
3. Add it to your `.env` file

### Google Maps API

1. Create a project in [Google Cloud Console](https://console.cloud.google.com/)
2. Enable the Maps JavaScript API
3. Create an API key
4. Add it to your `.env` file

---

## 📁 Project Structure

```
FINDHOPE/
├── src/
│   ├── components/        # Reusable UI components
│   ├── pages/            # Page components
│   ├── hooks/            # Custom React hooks
│   ├── integrations/     # Third-party integrations
│   ├── lib/              # Utility functions
│   ├── types/            # TypeScript type definitions
│   └── App.tsx           # Main application component
├── supabase/
│   └── functions/        # Edge functions for AI processing
├── public/               # Static assets
├── index.html            # HTML entry point
├── vite.config.ts        # Vite configuration
├── tailwind.config.ts    # Tailwind CSS configuration
└── package.json          # Project dependencies
```

---

## 🎨 Features in Detail

### Missing Person Reports

Users can submit comprehensive reports including:
- Personal details (name, age, gender, height, weight)
- Physical characteristics (hair color, eye color, distinguishing marks)
- Last known location with map integration
- Multiple photos for better matching
- Contact information

### Facial Recognition

AI-powered matching using:
- Advanced facial recognition algorithms
- Similarity scoring
- Batch processing of CCTV images
- Real-time match notifications

### CCTV Analysis

Upload and analyze CCTV footage:
- Image extraction from video
- Automated facial detection
- Cross-reference with missing person database
- Match percentage display

### Interactive Dashboard

Comprehensive case management:
- Active cases overview
- Recent matches
- Statistical insights
- Search and filter capabilities
- Export to PDF

---

## 🤝 Contributing

We welcome contributions to FINDHOPE! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Code Style

- Follow the existing code style
- Use TypeScript for all new components
- Write meaningful commit messages
- Add comments for complex logic
- Test your changes thoroughly

---

## 🐛 Bug Reports

Found a bug? Please open an issue with:
- A clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Your environment (OS, browser, Node version)

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 🙏 Acknowledgments

- **Hugging Face** - For providing facial recognition models
- **Supabase** - For the excellent backend platform
- **shadcn/ui** - For beautiful UI components
- **Radix UI** - For accessible primitives
- **The Open Source Community** - For amazing tools and libraries

---

## 📞 Contact & Support

- **GitHub Issues**: [Report a bug](https://github.com/bajrangi-IT/FINDHOPE/issues)
- **Repository**: [FINDHOPE](https://github.com/bajrangi-IT/FINDHOPE)

---

## 🌟 Star History

If you find this project useful, please consider giving it a star ⭐ on GitHub!

---

**Made with ❤️ to help reunite families**

---

## 📝 Changelog

### v1.0.0 (Initial Release)
- ✅ Missing person reporting system
- ✅ AI-powered facial recognition
- ✅ CCTV image analysis
- ✅ Interactive maps integration
- ✅ User authentication
- ✅ Responsive design
- ✅ PDF report generation
- ✅ Dashboard analytics

---

## 🗺️ Roadmap

- [ ] Mobile app (React Native)
- [ ] SMS/Email notifications
- [ ] Multi-language support
- [ ] Advanced analytics
- [ ] Integration with law enforcement databases
- [ ] Public awareness campaigns
- [ ] Volunteer coordination system
- [ ] Real-time chat support

---

**Together, we can bring hope to those who need it most.** 🙏
