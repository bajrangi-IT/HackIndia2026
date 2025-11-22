# 🔍 FINDHOPE - HackIndia 2026 Submission

**AI-Powered Missing Person Finder with Facial Recognition**

---

## 🏆 Hackathon Information

- **Event**: HackIndia 2026
- **Team Name**: FINDHOPE
- **Project Title**: FINDHOPE - Missing People Finder
- **Category**: Social Impact / AI & ML

---

## 👥 Team Members

| Name | GitHub Username | Role |
|------|----------------|------|
| [Member 1 Name] | [@github-username1](https://github.com/username1) | Full Stack Developer |
| [Member 2 Name] | [@github-username2](https://github.com/username2) | Frontend Developer |
| [Member 3 Name] | [@github-username3](https://github.com/username3) | Backend Developer |
| [Member 4 Name] | [@github-username4](https://github.com/username4) | UI/UX Designer |

> **Note**: Please update the team member information above

---

## 🌐 Live Demo

🔗 **Demo Link**: [https://find-hope.netlify.app/](https://find-hope.netlify.app/)

✅ **Live and fully functional!** Try it out to see the AI-powered facial recognition in action.

---

## 📖 Project Overview

**FINDHOPE** is a comprehensive missing person tracking application that leverages the power of AI and community collaboration to help reunite missing individuals with their families. The platform provides tools for reporting missing persons, uploading CCTV footage for facial recognition analysis, and maintaining a searchable database of cases.

### 💡 Problem Statement

Every year, thousands of people go missing, and families struggle to find them due to:
- Lack of centralized reporting systems
- Limited use of technology in search efforts
- Difficulty in processing CCTV footage manually
- No automated matching system across databases

### ✨ Our Solution

FINDHOPE addresses these challenges through:
- **AI-Powered Facial Recognition**: Automatically match photos with CCTV footage
- **Centralized Database**: Single platform for reporting and searching
- **Real-time Matching**: Instant notifications when potential matches are found
- **Community Support**: Enable families, volunteers, and authorities to collaborate

---

## 🎯 Key Features

- ✅ **Missing Person Reporting**: Comprehensive forms with photos and details
- ✅ **AI Facial Recognition**: Hugging Face-powered facial matching
- ✅ **CCTV Analysis**: Upload and analyze CCTV footage automatically
- ✅ **Interactive Maps**: Google Maps integration for location tracking
- ✅ **Real-time Matching**: Instant match notifications with similarity scores
- ✅ **Search & Filter**: Advanced search capabilities across database
- ✅ **Analytics Dashboard**: Comprehensive insights and case management
- ✅ **PDF Reports**: Generate and download detailed case reports
- ✅ **QR Code Sharing**: Easy case sharing via QR codes
- ✅ **Responsive Design**: Works on desktop, tablet, and mobile
- ✅ **Dark Mode**: User-friendly interface with theme support

---

## 🛠️ Tech Stack

### Frontend
- **React 18.3.1** - UI library
- **TypeScript 5.8.3** - Type safety
- **Vite 5.4.19** - Build tool
- **Tailwind CSS 3.4.17** - Styling
- **shadcn/ui** - Component library
- **Radix UI** - Accessible components

### Backend & Services
- **Supabase** - Database, Authentication, Storage
- **Supabase Edge Functions** - Serverless AI processing
- **Hugging Face API** - Facial recognition models

### Key Libraries
- React Router DOM - Routing
- TanStack React Query - Data fetching
- React Hook Form + Zod - Form validation
- Recharts - Data visualization
- Google Maps API - Location services
- jsPDF + html2canvas - PDF generation

---

## 🚀 How to Run

### Prerequisites
- Node.js v18 or higher
- npm or yarn
- Git

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/HackIndiaXYZ/HackIndia2026.git
   cd HackIndia2026/FINDHOPE
   ```

2. **Install dependencies**
   ```bash
   npm install
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
   
   Navigate to `http://localhost:5173`

### Build for Production
```bash
npm run build
npm run preview
```

---

## 📦 Supabase Setup (Optional for Local Testing)

If you want to run your own instance:

1. Create a Supabase project at [supabase.com](https://supabase.com/)
2. Run the SQL migrations from `supabase/migrations/`
3. Deploy Edge Functions:
   ```bash
   npm install -g supabase
   supabase login
   supabase link --project-ref your-project-ref
   supabase functions deploy match-photo
   supabase functions deploy process-cctv-image
   ```
4. Create storage buckets: `missing-persons-photos` and `cctv-images`

---

## 📁 Project Structure

```
trace-finder-link/
├── src/
│   ├── components/        # Reusable UI components
│   ├── pages/            # Page components
│   ├── hooks/            # Custom React hooks
│   ├── integrations/     # Third-party integrations
│   ├── lib/              # Utility functions
│   ├── types/            # TypeScript definitions
│   └── App.tsx           # Main app component
├── supabase/
│   └── functions/        # Edge functions for AI
├── public/               # Static assets
└── package.json          # Dependencies
```

---

## 🎥 Demo Workflow

1. **Report a Missing Person**: Fill out comprehensive form with photos
2. **AI Processing**: System analyzes facial features
3. **CCTV Upload**: Upload CCTV footage for analysis
4. **Automatic Matching**: AI compares faces and generates matches
5. **View Results**: See matches with similarity scores
6. **Download Report**: Generate PDF reports for sharing
7. **Share via QR**: Share case details via QR code

---

## 📊 Impact & Use Cases

### For Families
- Quick and easy reporting system
- Real-time updates on potential matches
- Access to comprehensive search database

### For Authorities
- Centralized missing person database
- Automated CCTV analysis
- Data-driven insights and analytics

### For Community
- Ability to help in search efforts
- Share information efficiently
- Collaborate with authorities

---

## 🌟 What Makes FINDHOPE Special

1. **AI-First Approach**: Leveraging cutting-edge facial recognition
2. **User-Centric Design**: Intuitive interface for all user groups
3. **Real-world Impact**: Solving a critical social problem
4. **Scalable Architecture**: Built to handle thousands of cases
5. **Open Source**: Community-driven development

---

## 🚧 Future Roadmap

- [ ] Mobile app (React Native)
- [ ] SMS/Email notifications
- [ ] Multi-language support
- [ ] Integration with law enforcement databases
- [ ] Real-time chat support
- [ ] Video analysis from CCTV
- [ ] Public awareness campaigns

---

## 🏅 Challenges We Faced

1. **Facial Recognition Accuracy**: Tuning AI models for diverse lighting and angles
2. **Performance Optimization**: Handling large image datasets efficiently
3. **Privacy Concerns**: Implementing secure data handling practices
4. **Real-time Processing**: Balancing speed with accuracy in matching

---

## 📝 Notes for Judges

- ✅ Fully functional prototype with AI integration
- ✅ Deployed and accessible via demo link
- ✅ Complete source code with documentation
- ✅ Addresses real-world social problem
- ✅ Built within hackathon timeline
- ✅ Scalable and production-ready architecture

---

## 📞 Contact & Links

- **Repository**: [GitHub](https://github.com/bajrangi-IT/FINDHOPE)
- **Demo**: [Live Demo](https://your-demo-link.com)
- **Documentation**: See README.md in project root

---

## 📄 License

MIT License - Feel free to use and modify

---

**Made with ❤️ for HackIndia 2026 - Together, we can bring hope to those who need it most.** 🙏
