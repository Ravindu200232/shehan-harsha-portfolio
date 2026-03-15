# 🚀 Advanced 3D Portfolio - Shehan Harsha Kumara
![image alt](https://github.com/ShehanHarshaKumara/shehan-harsha-portfolio/blob/Home/Screenshot%202026-03-15%20191407.png?raw=true)
![image alt](https://github.com/ShehanHarshaKumara/shehan-harsha-portfolio/blob/Home/Screenshot%202026-03-15%20191449.png?raw=true)
![image alt](https://github.com/ShehanHarshaKumara/shehan-harsha-portfolio/blob/Home/Screenshot%202026-03-15%20191550.png?raw=true)
A cutting-edge, modern portfolio website featuring advanced animations, 3D effects, and automatic GitHub integration.

## ✨ Features

### 🎨 Design & Animations
- **Typing Animation** - Dynamic name and role typing effect with cursor
- **Particle System** - Interactive particle network background
- **3D Tilt Effects** - Cards with parallax tilt on hover
- **Gradient Animations** - Smooth animated gradient backgrounds
- **Glassmorphism** - Modern frosted glass UI elements
- **Micro-interactions** - Polished hover states and transitions

### 🌓 Theme System
- **Dark/Light Mode** - Smooth theme switching with animations
- **Blue Color Scheme** - Consistent gradient theme throughout
- **Persistent Preferences** - Theme saved in localStorage

### 📱 Fully Responsive
- Mobile-first design approach
- Adaptive layouts for all screen sizes
- Touch-optimized interactions

### 🔗 GitHub Integration
- **Auto-Sync Projects** - Automatically fetches latest repos
- **Project Images** - Displays project screenshots
- **Live Stats** - Real-time stars, forks, and watchers
- **Language Badges** - Color-coded tech stack indicators

### 🎯 Sections

1. **Hero Section**
   - Particle background animation
   - Typing animation for name and roles
   - Animated gradient orbs
   - Social media links with hover effects
   - Smooth scroll indicator

2. **About Section**
   - 3D tilt cards
   - Feature highlights with gradient icons
   - Interactive stats cards
   - Engaging copy about experience

3. **Projects Section**
   - Tilt-enabled project cards
   - Auto-fetched from GitHub API
   - Project images from Unsplash
   - Live/GitHub links
   - Topic tags and stats

4. **Skills Section**
   - Animated progress bars with shine effects
   - Categorized by technology type
   - Icon-based visual hierarchy
   - Experience statistics

5. **Contact Section**
   - Working contact form
   - Glassmorphic design
   - Contact information cards
   - Form validation and loading states

6. **Navigation**
   - Sticky header with blur effect
   - Active section highlighting
   - Smooth scroll to sections
   - Mobile-responsive menu

## 🛠️ Tech Stack

- **React 18** - Latest React features
- **TypeScript** - Type-safe code
- **Tailwind CSS v4** - Modern utility-first CSS
- **Motion (Framer Motion)** - Advanced animations
- **React Type Animation** - Typing effects
- **React Parallax Tilt** - 3D card effects
- **Lucide React** - Beautiful icons
- **Sonner** - Toast notifications

## 🚀 Getting Started

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

### GitHub API Setup

To enable automatic project fetching from GitHub:

1. Open `/src/app/components/Projects.tsx`
2. Uncomment the GitHub API fetch code (around line 79)
3. Replace `ShehanHarshaKumara` with your GitHub username

#### Optional: Add GitHub Token for Higher Rate Limits

```typescript
fetch('https://api.github.com/users/YOUR_USERNAME/repos', {
  headers: {
    'Authorization': 'token YOUR_GITHUB_TOKEN'
  }
})
```

**Rate Limits:**
- Without token: 60 requests/hour
- With token: 5,000 requests/hour

### Customization

#### Update Personal Information

**Contact Details** (`/src/app/components/Contact.tsx`):
```typescript
const contactInfo = [
  { title: 'Email', value: 'your@email.com' },
  { title: 'Phone', value: '+1234567890' },
  { title: 'Location', value: 'Your City' },
];
```

**Social Links** (`/src/app/components/Hero.tsx`):
```typescript
{ icon: Github, href: 'https://github.com/yourusername' },
{ icon: Linkedin, href: 'https://linkedin.com/in/yourprofile' },
{ icon: Mail, href: 'mailto:your@email.com' },
```

#### Customize Skills

Edit `/src/app/components/Skills.tsx`:
```typescript
const skillCategories = [
  {
    category: 'Your Category',
    skills: [
      { name: 'Skill Name', level: 90, color: 'bg-blue-500' },
    ],
  },
];
```

#### Project Images

Projects automatically fetch themed images from Unsplash. To use real GitHub project images:

1. Add a social preview image to your GitHub repo:
   - Go to repo Settings > Options
   - Add a social preview image

2. Update the image URL in `Projects.tsx`:
```typescript
// Use GitHub's Open Graph image
const imageUrl = `https://opengraph.githubassets.com/[hash]/${owner}/${repo}`;
```

## 🎨 Color Scheme

The portfolio uses a sophisticated blue gradient theme:

- **Primary**: Blue (#3B82F6)
- **Secondary**: Cyan (#06B6D4)
- **Accent**: Purple (#A855F7)
- **Background**: Black with gradient overlays

## 📊 Performance

- **Optimized Animations** - GPU-accelerated transforms
- **Lazy Loading** - Images load on demand
- **Code Splitting** - Efficient bundle sizes
- **Smooth 60fps** - Butter-smooth animations

## 🌟 Unique Features

✅ **Interactive Particle Network** - Canvas-based particle system
✅ **Advanced Typing Effect** - Multiple roles with cursor animation  
✅ **3D Parallax Cards** - Tilt effect on project cards
✅ **Glassmorphism UI** - Modern frosted glass design
✅ **Smart Navigation** - Auto-highlights current section
✅ **GitHub Auto-Sync** - Live project updates
✅ **Form Validation** - Real-time input validation
✅ **Loading States** - Skeleton loaders and spinners
✅ **Toast Notifications** - User feedback system
✅ **SEO Optimized** - Semantic HTML structure

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Feel free to fork this project and customize it for your own portfolio!

## 💼 Credits

**Designed & Developed by:** Shehan Harsha Kumara  
**Portfolio:** [Your Portfolio URL]  
**GitHub:** [@ShehanHarshaKumara](https://github.com/ShehanHarshaKumara)

---

⭐ Star this repo if you found it helpful!
