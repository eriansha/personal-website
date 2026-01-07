# Personal Website Development Roadmap

**Created**: 2026-01-05
**Status**: Planning Phase
**Notation**: EARS (Easy Approach to Requirements Syntax)

---

## Executive Summary

This document provides an actionable roadmap for developing a personal website that showcases professional biography, portfolio work, and establishes a cohesive brand identity. The roadmap follows EARS notation for clear, unambiguous requirements.

---

## 1. Content Strategy

### 1.1 Site Structure

The website shall contain the following primary sections:

1. **Home/Landing Page**
   - The homepage shall display a hero section with name, tagline, and primary call-to-action
   - The homepage shall include navigation to all main sections
   - While on mobile devices, the homepage shall display a hamburger menu for navigation

2. **About/Biography**
   - The about page shall present professional background, skills, and personal story
   - The about page shall include education history and certifications
   - Where professional achievements exist, the about page shall display them prominently

3. **Portfolio/Work**
   - The portfolio page shall showcase projects with descriptions and visuals
   - When a portfolio item is selected, the system shall display a detailed case study
   - The portfolio page shall support filtering by category or technology

4. **Blog** (Optional)
   - Where blogging functionality exists, the blog shall display articles in reverse chronological order
   - The blog shall support categories and tags for organization

### 1.2 Content Requirements by Section

#### Homepage Content Needs

- Name and professional title
- Compelling tagline (10-15 words max)
- Brief value proposition (2-3 sentences)
- Social links and contact information
- Featured projects showcase
- **Note**: No personal photo required (text-based hero section)

#### Biography Content Needs

The biography section shall include:

- Professional summary (150-200 words)
- Core skills and competencies (8-12 items)
- Education background with degrees and institutions
- Career timeline with key positions
- Personal interests and values (humanizing element)
- Professional philosophy or mission statement

**Structure Recommendation**:

- When writing the biography, start with current role and work backwards
- The biography shall emphasize results and impact over responsibilities
- Where quantifiable achievements exist, the biography shall include specific metrics

#### Portfolio Content Needs

For each portfolio piece, the content shall include:

- Project title and subtitle
- Client/Company (if applicable)
- Role and responsibilities
- Project duration and timeline
- Problem statement
- Solution approach
- Technologies/tools used
- Key results and outcomes
- Visual assets (screenshots, mockups, photos)
- Link to live project (if available)

**Content Preparation Checklist**:

- [ ] Select 6-10 best representative projects
- [ ] Gather high-quality images for each project (minimum 1200px width)
- [ ] Write case studies following problem-solution-result structure
- [ ] Obtain client permission for public portfolio display
- [ ] Create project category taxonomy

---

## 2. Design Direction

### 2.1 Color Palette Strategy

The color scheme shall be selected based on industry and personal brand:

**For Tech/Engineering Field**:

- Primary: Deep blue (#0A2463) - Trust, professionalism
- Secondary: Vibrant cyan (#00B4D8) - Innovation, technology
- Accent: Warm orange (#F77F00) - Energy, creativity
- Neutral: Charcoal (#2B2D42) and Off-white (#F8F9FA)

**For Creative/Design Field**:

- Primary: Rich purple (#6A4C93) - Creativity, sophistication
- Secondary: Soft coral (#FF6B6B) - Warmth, approachability
- Accent: Golden yellow (#FFD23F) - Optimism, energy
- Neutral: Slate gray (#404E5C) and Cream (#FFFBF0)

**For Business/Consulting**:

- Primary: Navy (#1E3A5F) - Authority, reliability
- Secondary: Teal (#14B8A6) - Growth, balance
- Accent: Gold (#D4AF37) - Premium, success
- Neutral: Charcoal (#333333) and Light gray (#F5F5F5)

**Color Usage Requirements**:

- The design shall use the primary color for headers and key UI elements
- The design shall use the secondary color for links and interactive elements
- The design shall use the accent color sparingly for calls-to-action
- The design shall maintain WCAG AA contrast ratio (4.5:1) for all text

### 2.2 Typography

The typography system shall follow these requirements:

**Heading Font**:

- The website shall use a modern sans-serif for headings (e.g., Inter, Poppins, Montserrat)
- Heading font-weight shall be 600-700 for emphasis
- Where display headings exist, they shall use larger tracking (letter-spacing)

**Body Font**:

- The website shall use a readable serif or sans-serif for body text (e.g., Source Sans Pro, Open Sans, or Merriweather for serif)
- Body text shall be minimum 16px on mobile, 18px on desktop
- Line-height shall be 1.6-1.8 for optimal readability

**Type Scale**:

- The design shall implement a modular scale (1.25 or 1.333 ratio)
- When on mobile devices, the font sizes shall scale down proportionally

### 2.3 Layout Structure

**Grid System**:

- The layout shall use a 12-column grid on desktop
- When on tablet devices, the layout shall use an 8-column grid
- When on mobile devices, the layout shall use a 4-column grid
- The design shall maintain consistent gutter spacing (24px desktop, 16px mobile)

**Navigation**:

- The navigation shall be fixed at the top of the page
- While scrolling down, the navigation shall remain accessible
- When on mobile, the navigation shall collapse into a hamburger menu
- The navigation shall highlight the current section

**Section Layouts**:

- The homepage shall use full-width hero with centered content
- The about section shall use two-column layout (image + text) on desktop
- The portfolio shall use card-based grid layout (3 columns on desktop, 1 on mobile)
- Each section shall have adequate whitespace (minimum 80px vertical padding)

### 2.4 Imagery Style

The visual content shall follow these guidelines:

- All images shall be high-resolution (minimum 2x pixel density)
- The photography style shall be natural and authentic (avoid overly staged photos)
- When displaying project screenshots, they shall include device mockups for context
- Where illustrations are used, they shall maintain consistent style and color palette
- Profile photos shall be professionally shot with clean background

**Image Requirements**:

- Hero image: 1920x1080px minimum
- Portfolio images: 1200x800px minimum
- Profile photo: 800x800px minimum, square crop
- All images shall be optimized (WebP format with fallbacks)

---

## 3. Technical Considerations

### 3.1 Mobile Responsiveness

**Breakpoint Requirements**:

- The website shall support the following breakpoints:
  - Mobile: 320px - 767px
  - Tablet: 768px - 1023px
  - Desktop: 1024px - 1439px
  - Large Desktop: 1440px+

**Mobile-Specific Requirements**:

- When on mobile devices, touch targets shall be minimum 44x44px
- The website shall support touch gestures for portfolio galleries
- When on mobile, the website shall load mobile-optimized images
- The layout shall reflow content for single-column on mobile

### 3.2 Performance Optimization

**Loading Performance**:

- The website shall achieve Lighthouse performance score of 90+
- The initial page load shall complete in under 3 seconds on 3G
- When images are below the fold, the system shall lazy-load them
- The website shall implement critical CSS inlining for above-the-fold content

**Asset Optimization**:

- All images shall be compressed and served in next-gen formats (WebP, AVIF)
- The website shall implement responsive images with srcset
- JavaScript bundles shall be code-split by route
- The website shall use font-display: swap for web fonts

**Caching Strategy**:

- Static assets shall be cached with long expiration headers
- The website shall implement service worker for offline functionality (optional)

### 3.3 SEO Fundamentals

**Meta Tags**:

- Each page shall have a unique, descriptive title (50-60 characters)
- Each page shall have a meta description (150-160 characters)
- The website shall include Open Graph tags for social sharing
- The website shall include Twitter Card meta tags

**Content SEO**:

- The website shall use semantic HTML5 structure (header, nav, main, article, footer)
- Each page shall have one H1 tag
- The content shall use heading hierarchy (H1 → H2 → H3)
- All images shall have descriptive alt text

**Technical SEO**:

- The website shall include a sitemap.xml
- The website shall include a robots.txt file
- The website shall implement schema.org structured data for Person/Portfolio
- All links shall be crawlable (no JavaScript-only navigation)

**Performance as SEO**:

- Core Web Vitals shall meet "Good" thresholds:
  - LCP (Largest Contentful Paint): < 2.5s
  - FID (First Input Delay): < 100ms
  - CLS (Cumulative Layout Shift): < 0.1

---

## 4. Code Structure & Technical Architecture

### 4.1 Updated Feature Requirements

**Profile Context**: Full Stack Software Engineer with 8 years of experience across various tech stacks

**Main Features (P0 - Must Have for Launch)**:

1. **Home Page**
   - The homepage shall display name, professional title, and brief description (no photo required)
   - The homepage shall showcase featured projects in grid/card layout
   - The homepage shall include social links and contact information
   - The homepage shall use text animation for attention-grabbing effect (inspired by theodorusclarence.com)
   - The homepage shall establish clear personal branding with tagline/title

2. **About Page**
   - The about page shall display extended professional background
   - The about page shall include detailed work experience and skills
   - The about page shall present information not covered on homepage
   - The about page shall include career timeline or journey
   - The about page shall showcase technical stack expertise

3. **Projects/Portfolio Section**
   - Each project card shall display:
     - Project title
     - Short description
     - Project image/screenshot (if available)
     - Tech stack tags/badges
     - Live website link (if deployed)
     - GitHub repository link (if public)
   - The portfolio shall support filtering by technology or category
   - When a project is clicked, shall show detailed view or navigate to project page

**Nice-to-Have Features (P1 - Post Launch)**:

4. **Blog**
   - Where blog functionality exists, shall display articles with titles, excerpts, and dates
   - The blog shall support markdown or MDX content
   - The blog shall include reading time estimation
   - The blog shall support code syntax highlighting

5. **Code Snippets**
   - Where snippets feature exists, shall display reusable code examples
   - The snippets shall support multiple programming languages
   - The snippets shall include copy-to-clipboard functionality
   - The snippets shall support categorization by language/framework

**Creative Feature Suggestions (P2 - Future Enhancements)**:

6. **Command Palette** (inspired by cv.jarocki.me)
   - When `Cmd/Ctrl + K` or `Cmd/Ctrl + J` is pressed, the system shall open command palette
   - The command palette shall provide quick navigation shortcuts
   - The command palette shall support search functionality
   - The command palette shall include actions like "Copy email", "View resume", "Toggle theme"

7. **Interactive Timeline**
   - Visual career journey with milestones
   - Technology evolution over years
   - Project timeline view

8. **GitHub Activity Widget**
   - Display recent contributions
   - Show most popular repositories
   - Tech stack statistics from GitHub

9. **Now Page** (inspired by Derek Sivers)
   - What you're currently working on
   - Current learning focus
   - Recent reads/resources

### 4.2 Inspiration Sites Analysis

Based on the provided references, here's what to incorporate:

**1. [theodorusclarence.com](https://theodorusclarence.com/)**

- **Key Elements**:
  - Clean, minimal hero with animated text (name, title, description)
  - Elegant color tone (likely neutral with accent colors)
  - Smooth typography with hierarchy
- **Implementation Approach**:
  - Use Framer Motion for text animations (character-by-character reveal, fade-in)
  - Implement gradient text effects for name
  - Use Inter or similar modern sans-serif font
- **EARS Requirement**:
  - **ED-006**: When the homepage loads, the system shall animate the hero text with staggered fade-in effect

**2. [jackyef.com](https://jackyef.com/)**

- **Key Elements**:
  - Fun, playful color scheme
  - Name and description prominently displayed
  - Approachable personality through design
- **Implementation Approach**:
  - Use vibrant accent colors (possibly purple, blue, or teal)
  - Implement playful hover interactions
  - Add personality through micro-animations
- **EARS Requirement**:
  - **SD-005**: While hovering over interactive elements, the system shall display playful color transitions

**3. [cv.jarocki.me](https://cv.jarocki.me/)**

- **Key Elements**:
  - Command palette with `Cmd + J` shortcut
  - Quick actions and navigation
  - Keyboard-first interaction
- **Implementation Approach**:
  - Use `cmdk` library (Command Menu by Paco Coursey)
  - Implement global keyboard shortcuts
  - Provide actions: navigate, copy contact info, download resume, toggle theme
- **EARS Requirements**:
  - **ED-007**: When user presses `Cmd+K` or `Cmd+J`, the system shall open command palette overlay
  - **ED-008**: When user types in command palette, the system shall filter available commands
  - **ED-009**: When user selects a command, the system shall execute the corresponding action

**4. [faldi.xyz](https://faldi.xyz/)**

- **Key Elements**:
  - Straightforward branding: "Product Engineer & Mentor"
  - Portfolio structure with:
    - Title
    - Description
    - Image (optional)
    - Tech stack badges
    - Live link (if available)
    - GitHub link (if available)
- **Implementation Approach**:
  - Create `ProjectCard` component with consistent structure
  - Use tech stack badges/pills for visual scanning
  - Implement external link icons for live/GitHub links
  - Responsive grid layout (3 cols → 2 cols → 1 col)
- **EARS Requirement**:
  - **UR-006**: Each project card shall display title, description, optional image, tech stack, and available links (live/GitHub)

### 4.3 Recommended Tech Stack

**Current Setup**: React + Vite + TypeScript + Bun

**Additional Libraries**:

```json
{
  "dependencies": {
    "react": "^19.2.0",
    "react-dom": "^19.2.0",
    "@tanstack/react-router": "^1.x", // Type-safe routing
    "framer-motion": "^11.x", // Animations
    "cmdk": "^1.x", // Command palette
    "lucide-react": "^0.x", // Icons
    "class-variance-authority": "^0.7.x", // CVA for component variants
    "clsx": "^2.x", // Utility for classnames
    "tailwind-merge": "^2.x", // Merge Tailwind classes
    "zod": "^3.x" // Schema validation for search params
  },
  "devDependencies": {
    // ... existing dev dependencies
    "tailwindcss": "^4.x", // Utility-first CSS
    "autoprefixer": "^10.x",
    "postcss": "^8.x",
    "@tailwindcss/typography": "^0.5.x", // Blog typography
    "@tanstack/router-vite-plugin": "^1.x" // Router dev tools
  }
}
```

**Rationale**:

- **TanStack Router**: Type-safe routing with excellent TypeScript support, built-in code splitting, search params validation
- **shadcn/ui**: Not a dependency but a collection of copy-paste components built with Radix UI and Tailwind
- **Framer Motion**: Declarative animations, excellent performance, great DX
- **cmdk**: Best-in-class command palette (used by Linear, Vercel, etc.)
- **Lucide React**: Modern icon set, tree-shakeable, consistent design
- **Tailwind CSS**: Utility-first CSS framework, rapid development, excellent performance
- **CVA**: Type-safe component variants (used by shadcn/ui)

**shadcn/ui Setup**:

```bash
# Initialize shadcn/ui
bunx shadcn@latest init

# Add components as needed
bunx shadcn@latest add button
bunx shadcn@latest add card
bunx shadcn@latest add badge
bunx shadcn@latest add dropdown-menu
bunx shadcn@latest add dialog
bunx shadcn@latest add tooltip
```

**Alternative Considerations**:

- **Routing**: TanStack Router provides better TypeScript experience than React Router
- **UI Components**: shadcn/ui provides accessible components you own (not a dependency)
- **Animations**: Could use GSAP for complex animations, but Framer Motion sufficient for most needs
- **Markdown**: Add `react-markdown` + `remark-gfm` for blog (P1)
- **Syntax Highlighting**: Add `shiki` or `prism-react-renderer` for code blocks (P1)

### 4.4 Project File Structure

```
personal-website/
├── public/
│   ├── projects/              # Project images/screenshots
│   ├── favicon.ico
│   └── robots.txt
├── src/
│   ├── assets/                # Static assets
│   │   └── icons/
│   ├── components/            # Reusable components
│   │   ├── ui/               # shadcn/ui components (auto-generated)
│   │   │   ├── button.tsx
│   │   │   ├── card.tsx
│   │   │   ├── badge.tsx
│   │   │   ├── dialog.tsx
│   │   │   ├── dropdown-menu.tsx
│   │   │   └── tooltip.tsx
│   │   ├── layout/           # Layout components
│   │   │   ├── Header.tsx
│   │   │   ├── Footer.tsx
│   │   │   ├── Navigation.tsx
│   │   │   └── RootLayout.tsx
│   │   ├── home/             # Home page components
│   │   │   ├── Hero.tsx
│   │   │   ├── FeaturedProjects.tsx
│   │   │   └── SocialLinks.tsx
│   │   ├── projects/         # Project components
│   │   │   ├── ProjectCard.tsx
│   │   │   ├── ProjectGrid.tsx
│   │   │   ├── ProjectFilter.tsx
│   │   │   └── TechBadge.tsx
│   │   ├── about/            # About page components
│   │   │   ├── Timeline.tsx
│   │   │   ├── Skills.tsx
│   │   │   └── Experience.tsx
│   │   └── shared/           # Shared components
│   │       ├── CommandPalette.tsx
│   │       ├── ThemeToggle.tsx
│   │       └── AnimatedText.tsx
│   ├── data/                 # Static data & content
│   │   ├── projects.ts       # Projects data
│   │   ├── experience.ts     # Work experience
│   │   ├── skills.ts         # Skills & technologies
│   │   ├── social.ts         # Social links
│   │   └── site-config.ts    # Site metadata
│   ├── hooks/                # Custom React hooks
│   │   ├── useKeyboardShortcut.ts
│   │   ├── useTheme.ts
│   │   └── useScrollPosition.ts
│   ├── lib/                  # Utility functions
│   │   ├── utils.ts          # cn() utility and helpers
│   │   └── constants.ts
│   ├── routes/               # TanStack Router routes
│   │   ├── __root.tsx        # Root route with layout
│   │   ├── index.tsx         # Home page (/)
│   │   ├── about.tsx         # About page (/about)
│   │   ├── projects.tsx      # Projects page (/projects)
│   │   └── projects.$id.tsx  # Project detail (/projects/$id)
│   ├── styles/               # Global styles
│   │   ├── globals.css
│   │   └── animations.css
│   ├── types/                # TypeScript types
│   │   ├── project.ts
│   │   ├── experience.ts
│   │   └── index.ts
│   ├── main.tsx              # Entry point with router setup
│   ├── routeTree.gen.ts      # Auto-generated route tree
│   ├── vite-env.d.ts
│   └── components.json       # shadcn/ui config
├── .prettierrc
├── eslint.config.js
├── tailwind.config.js
├── tsconfig.json
├── vite.config.ts
└── package.json
```

**File Structure Principles**:

- **Co-location**: Components grouped by feature/page
- **Separation of Concerns**: Data, UI, logic separated
- **File-based Routing**: TanStack Router uses file-based routes in `src/routes/`
- **shadcn/ui Components**: UI primitives in `src/components/ui/` (generated via CLI)
- **Scalability**: Easy to add new features (blog, snippets)
- **Type Safety**: Strong typing with TypeScript + TanStack Router

### 4.5 Data Management Strategy

**Approach**: Static Data (JSON/TypeScript) → No Database Required

For a personal portfolio with infrequent updates, static data files are sufficient and provide:

- Type safety with TypeScript
- Version control for content changes
- Fast builds and performance
- Simple deployment (no backend needed)

**Example: `src/data/projects.ts`**

```typescript
export interface Project {
  id: string
  title: string
  description: string
  longDescription?: string // For detail page
  image?: string // Path to project image
  techStack: string[] // Array of technologies
  liveUrl?: string // Deployed website URL
  githubUrl?: string // GitHub repository URL
  featured: boolean // Show on homepage
  category: ProjectCategory
  startDate: string // ISO date
  endDate?: string // ISO date, optional for ongoing
}

export type ProjectCategory =
  | 'web-app'
  | 'mobile-app'
  | 'api'
  | 'library'
  | 'tool'
  | 'open-source'

export const projects: Project[] = [
  {
    id: 'ecommerce-platform',
    title: 'E-Commerce Platform',
    description: 'Scalable multi-vendor marketplace with real-time inventory',
    longDescription: '...',
    image: '/projects/ecommerce.png',
    techStack: ['React', 'Node.js', 'PostgreSQL', 'Redis', 'Docker'],
    liveUrl: 'https://example.com',
    githubUrl: 'https://github.com/username/repo',
    featured: true,
    category: 'web-app',
    startDate: '2023-01-15',
    endDate: '2023-06-30',
  },
  // ... more projects
]

// Helper functions
export const getFeaturedProjects = () => projects.filter(p => p.featured)

export const getProjectsByCategory = (category: ProjectCategory) =>
  projects.filter(p => p.category === category)

export const getAllTechStack = () =>
  Array.from(new Set(projects.flatMap(p => p.techStack))).sort()
```

**Benefits**:

- Type-safe data access
- Easy to query and filter
- Can migrate to CMS later if needed (Contentful, Sanity, etc.)
- Version controlled content

**For Blog (P1)**:

- Use markdown files in `content/blog/` directory
- Use Vite plugins to import markdown as modules
- Or use a headless CMS (Contentful, Strapi) for easier editing

### 4.6 Component Architecture

**Design System Approach**: shadcn/ui + Atomic Design Lite

**Base Components (shadcn/ui)** - `src/components/ui/`

shadcn/ui provides accessible, customizable components built with Radix UI and Tailwind CSS. These are copy-pasted into your project (not installed as dependencies), giving you full control.

```typescript
// Generated via: bunx shadcn@latest add button
// src/components/ui/button.tsx
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { cva, type VariantProps } from "class-variance-authority"
import { cn } from "@/lib/utils"

const buttonVariants = cva(
  "inline-flex items-center justify-center rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-2 disabled:pointer-events-none disabled:opacity-50",
  {
    variants: {
      variant: {
        default: "bg-primary text-primary-foreground hover:bg-primary/90",
        destructive: "bg-destructive text-destructive-foreground hover:bg-destructive/90",
        outline: "border border-input bg-background hover:bg-accent hover:text-accent-foreground",
        secondary: "bg-secondary text-secondary-foreground hover:bg-secondary/80",
        ghost: "hover:bg-accent hover:text-accent-foreground",
        link: "text-primary underline-offset-4 hover:underline",
      },
      size: {
        default: "h-10 px-4 py-2",
        sm: "h-9 rounded-md px-3",
        lg: "h-11 rounded-md px-8",
        icon: "h-10 w-10",
      },
    },
    defaultVariants: {
      variant: "default",
      size: "default",
    },
  }
)

export interface ButtonProps
  extends React.ButtonHTMLAttributes<HTMLButtonElement>,
    VariantProps<typeof buttonVariants> {
  asChild?: boolean
}

export const Button = React.forwardRef<HTMLButtonElement, ButtonProps>(
  ({ className, variant, size, asChild = false, ...props }, ref) => {
    const Comp = asChild ? Slot : "button"
    return (
      <Comp
        className={cn(buttonVariants({ variant, size, className }))}
        ref={ref}
        {...props}
      />
    )
  }
)
```

**Utility Functions** - `src/lib/utils.ts`

```typescript
import { type ClassValue, clsx } from 'clsx'
import { twMerge } from 'tailwind-merge'

// Merge Tailwind classes without conflicts
export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs))
}
```

**Feature Components** - `src/components/projects/`

```typescript
// ProjectCard.tsx
import { Project } from '@/types/project'
import { Card, CardHeader, CardTitle, CardDescription, CardContent, CardFooter } from '@/components/ui/card'
import { Badge } from '@/components/ui/badge'
import { Button } from '@/components/ui/button'
import { Github, ExternalLink } from 'lucide-react'

interface ProjectCardProps {
  project: Project
  layout?: 'grid' | 'list'
}

export function ProjectCard({ project, layout = 'grid' }: ProjectCardProps) {
  return (
    <Card className="group hover:shadow-lg transition-shadow">
      {project.image && (
        <img
          src={project.image}
          alt={project.title}
          className="w-full h-48 object-cover rounded-t-lg"
        />
      )}

      <CardHeader>
        <CardTitle>{project.title}</CardTitle>
        <CardDescription>{project.description}</CardDescription>
      </CardHeader>

      <CardContent>
        <div className="flex flex-wrap gap-2">
          {project.techStack.map(tech => (
            <Badge key={tech} variant="secondary">
              {tech}
            </Badge>
          ))}
        </div>
      </CardContent>

      <CardFooter className="gap-2">
        {project.liveUrl && (
          <Button variant="default" size="sm" asChild>
            <a href={project.liveUrl} target="_blank" rel="noopener noreferrer">
              <ExternalLink className="mr-2 h-4 w-4" />
              Live
            </a>
          </Button>
        )}
        {project.githubUrl && (
          <Button variant="outline" size="sm" asChild>
            <a href={project.githubUrl} target="_blank" rel="noopener noreferrer">
              <Github className="mr-2 h-4 w-4" />
              Code
            </a>
          </Button>
        )}
      </CardFooter>
    </Card>
  )
}
```

**Animation Wrapper Pattern**:

```typescript
// components/shared/AnimatedText.tsx
import { motion } from 'framer-motion'

interface AnimatedTextProps {
  text: string
  variant?: 'fadeIn' | 'slideUp' | 'typewriter'
  delay?: number
}

export function AnimatedText({ text, variant = 'fadeIn', delay = 0 }: AnimatedTextProps) {
  const variants = {
    fadeIn: {
      initial: { opacity: 0 },
      animate: { opacity: 1 },
      transition: { duration: 0.6, delay }
    },
    slideUp: {
      initial: { opacity: 0, y: 20 },
      animate: { opacity: 1, y: 0 },
      transition: { duration: 0.5, delay }
    }
  }

  return (
    <motion.div {...variants[variant]}>
      {text}
    </motion.div>
  )
}
```

### 4.7 Routing Strategy

**File-Based Routing with TanStack Router**

TanStack Router provides type-safe, file-based routing with excellent TypeScript support and built-in code splitting.

**Vite Configuration** - `vite.config.ts`

```typescript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import { TanStackRouterVite } from '@tanstack/router-vite-plugin'

export default defineConfig({
  plugins: [
    react(),
    TanStackRouterVite(), // Auto-generates routeTree.gen.ts
  ],
  resolve: {
    alias: {
      '@': '/src',
    },
  },
})
```

**Root Route** - `src/routes/__root.tsx`

```typescript
import { createRootRoute, Outlet } from '@tanstack/react-router'
import { TanStackRouterDevtools } from '@tanstack/router-devtools'
import { Header } from '@/components/layout/Header'
import { Footer } from '@/components/layout/Footer'
import { CommandPalette } from '@/components/shared/CommandPalette'

export const Route = createRootRoute({
  component: RootLayout,
})

function RootLayout() {
  return (
    <>
      <CommandPalette />
      <Header />
      <main className="min-h-screen">
        <Outlet />
      </main>
      <Footer />
      {process.env.NODE_ENV === 'development' && <TanStackRouterDevtools />}
    </>
  )
}
```

**Home Route** - `src/routes/index.tsx`

```typescript
import { createFileRoute } from '@tanstack/react-router'
import { Hero } from '@/components/home/Hero'
import { FeaturedProjects } from '@/components/home/FeaturedProjects'
import { SocialLinks } from '@/components/home/SocialLinks'

export const Route = createFileRoute('/')({
  component: HomePage,
  meta: () => [
    { title: 'Ivan Putra Eriansya | Full Stack Software Engineer' },
    { name: 'description', content: 'Full Stack Engineer with 8 years of experience...' },
  ],
})

function HomePage() {
  return (
    <div className="container mx-auto px-4">
      <Hero />
      <FeaturedProjects />
      <SocialLinks />
    </div>
  )
}
```

**About Route** - `src/routes/about.tsx`

```typescript
import { createFileRoute } from '@tanstack/react-router'
import { Timeline } from '@/components/about/Timeline'
import { Skills } from '@/components/about/Skills'

export const Route = createFileRoute('/about')({
  component: AboutPage,
})

function AboutPage() {
  return (
    <div className="container mx-auto px-4 py-12">
      <h1 className="text-4xl font-bold mb-8">About Me</h1>
      <Timeline />
      <Skills />
    </div>
  )
}
```

**Projects Route with Search Params** - `src/routes/projects.tsx`

```typescript
import { createFileRoute } from '@tanstack/react-router'
import { z } from 'zod'
import { ProjectGrid } from '@/components/projects/ProjectGrid'
import { ProjectFilter } from '@/components/projects/ProjectFilter'

// Type-safe search params
const projectSearchSchema = z.object({
  category: z.string().optional(),
  tech: z.string().optional(),
})

export const Route = createFileRoute('/projects')({
  component: ProjectsPage,
  validateSearch: projectSearchSchema,
})

function ProjectsPage() {
  const { category, tech } = Route.useSearch()

  return (
    <div className="container mx-auto px-4 py-12">
      <h1 className="text-4xl font-bold mb-8">Projects</h1>
      <ProjectFilter />
      <ProjectGrid category={category} tech={tech} />
    </div>
  )
}
```

**Project Detail Route (Dynamic)** - `src/routes/projects.$id.tsx`

```typescript
import { createFileRoute, notFound } from '@tanstack/react-router'
import { projects } from '@/data/projects'

export const Route = createFileRoute('/projects/$id')({
  component: ProjectDetailPage,
  loader: ({ params }) => {
    const project = projects.find(p => p.id === params.id)
    if (!project) throw notFound()
    return { project }
  },
})

function ProjectDetailPage() {
  const { project } = Route.useLoaderData()

  return (
    <div className="container mx-auto px-4 py-12">
      <h1 className="text-4xl font-bold mb-4">{project.title}</h1>
      <p className="text-lg text-muted-foreground">{project.description}</p>
      {/* Project details */}
    </div>
  )
}
```

**Main Entry Point** - `src/main.tsx`

```typescript
import React from 'react'
import ReactDOM from 'react-dom/client'
import { RouterProvider, createRouter } from '@tanstack/react-router'
import { routeTree } from './routeTree.gen' // Auto-generated
import './styles/globals.css'

// Create router instance
const router = createRouter({
  routeTree,
  defaultPreload: 'intent', // Preload on hover
})

// Type-safe router for global use
declare module '@tanstack/react-router' {
  interface Register {
    router: typeof router
  }
}

ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <RouterProvider router={router} />
  </React.StrictMode>
)
```

**Benefits**:

- **Type Safety**: Full TypeScript support with autocomplete for routes and params
- **File-Based**: Routes automatically generated from file structure
- **Code Splitting**: Automatic code splitting by route
- **Search Params Validation**: Type-safe search/query parameters with Zod
- **Data Loaders**: Load data before rendering (similar to Remix/Next.js)
- **Preloading**: Intelligent route preloading on hover
- **DevTools**: Built-in router devtools for development
- **No Manual Route Config**: Routes auto-generated from file names

### 4.8 Animation Implementation

**Framer Motion Best Practices**

**1. Page Transitions**:

```typescript
// pages/HomePage.tsx
import { motion } from 'framer-motion'

const pageVariants = {
  initial: { opacity: 0, y: 20 },
  animate: {
    opacity: 1,
    y: 0,
    transition: { duration: 0.5, ease: 'easeOut' }
  },
  exit: {
    opacity: 0,
    transition: { duration: 0.3 }
  }
}

export function HomePage() {
  return (
    <motion.div
      variants={pageVariants}
      initial="initial"
      animate="animate"
      exit="exit"
    >
      {/* Page content */}
    </motion.div>
  )
}
```

**2. Staggered Children (for project grid)**:

```typescript
const containerVariants = {
  hidden: { opacity: 0 },
  visible: {
    opacity: 1,
    transition: {
      staggerChildren: 0.1 // Delay between each child
    }
  }
}

const itemVariants = {
  hidden: { opacity: 0, y: 20 },
  visible: { opacity: 1, y: 0 }
}

<motion.div
  variants={containerVariants}
  initial="hidden"
  animate="visible"
  className="project-grid"
>
  {projects.map(project => (
    <motion.div key={project.id} variants={itemVariants}>
      <ProjectCard project={project} />
    </motion.div>
  ))}
</motion.div>
```

**3. Text Animation (inspired by theodorusclarence.com)**:

```typescript
// Hero text with character animation
import { motion } from 'framer-motion'

const text = "Full Stack Software Engineer"

const containerVariants = {
  hidden: { opacity: 0 },
  visible: {
    opacity: 1,
    transition: { staggerChildren: 0.03 }
  }
}

const charVariants = {
  hidden: { opacity: 0, y: 10 },
  visible: { opacity: 1, y: 0 }
}

<motion.h1 variants={containerVariants} initial="hidden" animate="visible">
  {text.split('').map((char, i) => (
    <motion.span key={i} variants={charVariants}>
      {char}
    </motion.span>
  ))}
</motion.h1>
```

**4. Hover Interactions**:

```typescript
<motion.div
  whileHover={{ scale: 1.03, y: -5 }}
  whileTap={{ scale: 0.98 }}
  transition={{ type: 'spring', stiffness: 300 }}
>
  <ProjectCard {...props} />
</motion.div>
```

**Performance Considerations**:

- Use `will-change` CSS property sparingly
- Animate transforms and opacity (GPU accelerated)
- Avoid animating layout properties (width, height, padding)
- Use `useReducedMotion` hook for accessibility

### 4.9 Command Palette Implementation

**Using `cmdk` library** (inspired by cv.jarocki.me)

```typescript
// components/shared/CommandPalette.tsx
import { useEffect, useState } from 'react'
import { useNavigate } from '@tanstack/react-router'
import { Command } from 'cmdk'
import {
  Home, User, Briefcase, Mail, Github,
  Linkedin, FileText
} from 'lucide-react'
import { Dialog, DialogContent } from '@/components/ui/dialog'

export function CommandPalette() {
  const [open, setOpen] = useState(false)
  const navigate = useNavigate()

  // Keyboard shortcut: Cmd+K or Cmd+J
  useEffect(() => {
    const down = (e: KeyboardEvent) => {
      if ((e.key === 'k' || e.key === 'j') && (e.metaKey || e.ctrlKey)) {
        e.preventDefault()
        setOpen((open) => !open)
      }
    }
    document.addEventListener('keydown', down)
    return () => document.removeEventListener('keydown', down)
  }, [])

  const runCommand = (command: () => void) => {
    setOpen(false)
    command()
  }

  return (
    <Dialog open={open} onOpenChange={setOpen}>
      <DialogContent className="overflow-hidden p-0">
        <Command className="[&_[cmdk-group-heading]]:px-2 [&_[cmdk-group-heading]]:font-medium [&_[cmdk-group-heading]]:text-muted-foreground">
          <Command.Input
            placeholder="Type a command or search..."
            className="h-12 px-4 text-sm outline-none"
          />
          <Command.List className="max-h-[300px] overflow-y-auto p-2">
            <Command.Empty>No results found.</Command.Empty>

            <Command.Group heading="Navigation">
              <Command.Item
                onSelect={() => runCommand(() => navigate({ to: '/' }))}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <Home size={16} />
                <span>Home</span>
              </Command.Item>
              <Command.Item
                onSelect={() => runCommand(() => navigate({ to: '/about' }))}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <User size={16} />
                <span>About</span>
              </Command.Item>
              <Command.Item
                onSelect={() => runCommand(() => navigate({ to: '/projects' }))}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <Briefcase size={16} />
                <span>Projects</span>
              </Command.Item>
            </Command.Group>

            <Command.Group heading="Actions">
              <Command.Item
                onSelect={() => runCommand(() => {
                  navigator.clipboard.writeText('eriansha.van@gmail.com')
                })}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <Mail size={16} />
                <span>Copy Email</span>
              </Command.Item>
              <Command.Item
                onSelect={() => runCommand(() => {
                  window.open('/resume.pdf', '_blank')
                })}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <FileText size={16} />
                <span>Download Resume</span>
              </Command.Item>
            </Command.Group>

            <Command.Group heading="Social">
              <Command.Item
                onSelect={() => runCommand(() => {
                  window.open('https://github.com/eriansha', '_blank')
                })}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <Github size={16} />
                <span>GitHub</span>
              </Command.Item>
              <Command.Item
                onSelect={() => runCommand(() => {
                  window.open('https://linkedin.com/in/eriansha', '_blank')
                })}
                className="flex items-center gap-2 rounded-sm px-2 py-1.5 text-sm hover:bg-accent cursor-pointer"
              >
                <Linkedin size={16} />
                <span>LinkedIn</span>
              </Command.Item>
            </Command.Group>
          </Command.List>
        </Command>
      </DialogContent>
    </Dialog>
  )
}
```

**Features**:

- `Cmd+K` or `Cmd+J` to open
- Fuzzy search
- Keyboard navigation
- Quick actions (copy email, download resume, toggle theme)
- Navigation shortcuts
- Extensible for future commands

**EARS Requirements**:

- **ED-007**: When user presses `Cmd+K` or `Cmd+J`, the system shall open command palette
- **ED-008**: When user types in command palette, the system shall filter commands with fuzzy matching
- **ED-009**: When command is selected, the system shall execute action and close palette

### 4.10 Theme System (Dark Mode)

**Tailwind CSS with CSS Variables**

```typescript
// hooks/useTheme.ts
import { useEffect, useState } from 'react'

type Theme = 'light' | 'dark'

export function useTheme() {
  const [theme, setTheme] = useState<Theme>(() => {
    // Check localStorage or system preference
    const stored = localStorage.getItem('theme') as Theme
    if (stored) return stored

    return window.matchMedia('(prefers-color-scheme: dark)').matches
      ? 'dark'
      : 'light'
  })

  useEffect(() => {
    const root = document.documentElement
    root.classList.remove('light', 'dark')
    root.classList.add(theme)
    localStorage.setItem('theme', theme)
  }, [theme])

  const toggleTheme = () => {
    setTheme(prev => (prev === 'light' ? 'dark' : 'light'))
  }

  return { theme, toggleTheme }
}
```

**Tailwind Configuration**:

```javascript
// tailwind.config.js
module.exports = {
  darkMode: 'class',
  theme: {
    extend: {
      colors: {
        // Define color variables that work in both themes
        background: 'var(--background)',
        foreground: 'var(--foreground)',
        primary: 'var(--primary)',
        secondary: 'var(--secondary)',
        accent: 'var(--accent)',
      },
    },
  },
}
```

**CSS Variables** (globals.css):

```css
:root {
  --background: 255 255 255;
  --foreground: 0 0 0;
  --primary: 10 36 99; /* Deep blue */
  --secondary: 0 180 216; /* Cyan */
  --accent: 247 127 0; /* Orange */
}

.dark {
  --background: 15 23 42; /* slate-900 */
  --foreground: 248 250 252; /* slate-50 */
  --primary: 96 165 250; /* blue-400 */
  --secondary: 34 211 238; /* cyan-400 */
  --accent: 251 146 60; /* orange-400 */
}
```

### 4.11 SEO & Meta Tags Strategy

**React Helmet Async** for dynamic meta tags

```typescript
// components/shared/SEO.tsx
import { Helmet } from 'react-helmet-async'

interface SEOProps {
  title: string
  description: string
  image?: string
  url?: string
  type?: 'website' | 'article'
}

export function SEO({
  title,
  description,
  image = '/og-image.png',
  url,
  type = 'website'
}: SEOProps) {
  const siteTitle = 'Muhamad Eriansya | Full Stack Engineer'
  const fullTitle = title ? `${title} | ${siteTitle}` : siteTitle
  const fullUrl = url || window.location.href

  return (
    <Helmet>
      <title>{fullTitle}</title>
      <meta name="description" content={description} />

      {/* Open Graph */}
      <meta property="og:type" content={type} />
      <meta property="og:title" content={fullTitle} />
      <meta property="og:description" content={description} />
      <meta property="og:image" content={image} />
      <meta property="og:url" content={fullUrl} />

      {/* Twitter */}
      <meta name="twitter:card" content="summary_large_image" />
      <meta name="twitter:title" content={fullTitle} />
      <meta name="twitter:description" content={description} />
      <meta name="twitter:image" content={image} />
    </Helmet>
  )
}
```

**Usage in Pages**:

```typescript
export function HomePage() {
  return (
    <>
      <SEO
        title="Home"
        description="Full Stack Software Engineer with 8 years of experience building scalable web applications"
      />
      {/* Page content */}
    </>
  )
}
```

### 4.12 Development Workflow

**1. Local Development**:

```bash
# Start dev server
bun run dev

# Run linter
bun run lint

# Format code
bun run format

# Type check
bun run type-check  # Add to package.json: "tsc --noEmit"
```

**2. Build & Preview**:

```bash
# Build for production
bun run build

# Preview production build
bun run preview
```

**3. Code Quality Checks** (add to package.json):

```json
{
  "scripts": {
    "dev": "bunx --bun vite",
    "build": "tsc -b && bunx --bun vite build",
    "preview": "bunx --bun vite preview",
    "lint": "eslint .",
    "format": "prettier --write .",
    "format:check": "prettier --check .",
    "type-check": "tsc --noEmit"
  }
}
```

**4. Git Hooks** (optional, using husky):

- Pre-commit: Run lint + format check
- Pre-push: Run type-check + build

### 4.13 Deployment Strategy

**Recommended Platforms** (all support Bun now):

1. **Vercel** (Recommended)
   - Zero config deployment
   - Automatic previews for PRs
   - Edge functions support
   - Excellent performance

2. **Netlify**
   - Simple deployment
   - Form handling built-in
   - Good CDN

3. **Cloudflare Pages**
   - Fast global CDN
   - Free tier generous
   - Edge runtime

**Deployment Steps** (Vercel example):

```bash
# Install Vercel CLI
bun add -g vercel

# Deploy
vercel

# Production deployment
vercel --prod
```

**Environment Variables** (if needed):

```bash
# .env.example
VITE_SITE_URL=https://yoursite.com
VITE_CONTACT_EMAIL=your.email@example.com
# Add any API keys for analytics, etc.
```

### 4.14 Implementation Roadmap (Updated)

**Phase 1: Foundation** (Week 1)

- [ ] Set up Tailwind CSS with animations
- [ ] Initialize shadcn/ui (`bunx shadcn@latest init`)
- [ ] Install additional dependencies (@tanstack/react-router, framer-motion, cmdk, lucide-react)
- [ ] Add shadcn/ui components (button, card, badge, dialog, dropdown-menu, tooltip)
- [ ] Set up TanStack Router with Vite plugin
- [ ] Create route files structure in `src/routes/`
- [ ] Create Layout component in `__root.tsx` (Header, Footer)
- [ ] Implement theme system (light/dark mode) with shadcn/ui
- [ ] Set up global styles and CSS variables
- [ ] Configure path aliases (@/ for src) in tsconfig and vite.config

**Phase 2: Data & Content** (Week 1-2)

- [ ] Create type definitions (Project, Experience, Skill)
- [ ] Populate `data/projects.ts` with portfolio projects
- [ ] Populate `data/experience.ts` with work history
- [ ] Populate `data/skills.ts` with tech stack
- [ ] Write homepage copy (name, title, description)
- [ ] Write about page content

**Phase 3: Core Pages** (Week 2-3)

- [ ] Build HomePage (src/routes/index.tsx)
  - Hero section with animated text
  - Featured projects grid
  - Social links
- [ ] Build AboutPage (src/routes/about.tsx)
  - Extended bio
  - Timeline/Experience section
  - Skills showcase
- [ ] Build ProjectsPage (src/routes/projects.tsx)
  - Full project grid with filtering
  - Project cards with all fields
- [ ] Build ProjectDetailPage (src/routes/projects.$id.tsx)
  - Individual project showcase

**Phase 4: Enhanced Features** (Week 3-4)

- [ ] Implement Command Palette (Cmd+K)
- [ ] Add page transitions with Framer Motion
- [ ] Add micro-interactions (hover effects, loading states)
- [ ] Implement ProjectCard with proper structure (inspired by faldi.xyz)
- [ ] Add 404 page
- [ ] SEO optimization (meta tags, OpenGraph, sitemap)

**Phase 5: Polish** (Week 4)

- [ ] Performance optimization
- [ ] Accessibility audit
- [ ] Cross-browser testing
- [ ] Mobile responsiveness testing
- [ ] Add loading skeletons
- [ ] Deploy to production

**Phase 6: Post-Launch** (P1 Features)

- [ ] Blog functionality (markdown-based)
- [ ] Snippets section
- [ ] Analytics integration
- [ ] RSS feed
- [ ] Newsletter signup (optional)

### 4.15 Additional EARS Requirements for Code Structure

**Component Requirements**:

**UR-007**: All components shall be typed with TypeScript interfaces

**UR-008**: All external links shall open in new tab with `rel="noopener noreferrer"`

**UR-009**: All images shall include alt text for accessibility

**SD-006**: While theme is 'dark', all components shall use dark mode color variables

**ED-010**: When project tech badge is clicked, the system shall filter projects by that technology

**ED-011**: When external link is hovered, the system shall display tooltip with full URL

**OF-004**: Where command palette is implemented, the system shall support custom keyboard shortcuts

**OF-005**: Where animations are implemented, the system shall respect `prefers-reduced-motion`

**UB-005**: If component fails to render, the system shall display error boundary with recovery option

---

## 5. Timeline & Milestones

### Phase 1: Planning & Content Preparation (2-3 weeks)

**Must-Have**:

- [ ] Finalize site structure and page list
- [ ] Write all biography content
- [ ] Select and prepare portfolio projects (6-10)
- [ ] Gather all visual assets
- [ ] Define brand colors and typography

**Nice-to-Have**:

- [ ] Create content calendar for blog
- [ ] Professional photoshoot
- [ ] Video introduction

**Deliverables**:

- Content document with all copy
- Asset library (images, logos, files)
- Brand style guide

### Phase 2: Design & Prototyping (2-3 weeks)

**Must-Have**:

- [ ] Create wireframes for all pages (mobile + desktop)
- [ ] Design high-fidelity mockups for homepage and about page
- [ ] Design portfolio grid and case study template
- [ ] Establish component library (buttons, cards, forms)

**Nice-to-Have**:

- [ ] Interactive prototype in Figma
- [ ] Micro-interactions and animations design
- [ ] Dark mode design variant

**Deliverables**:

- Design files (Figma/Sketch)
- Component specifications
- Design system documentation

### Phase 3: Development - Core Features (3-4 weeks)

**Must-Have**:

- [ ] Set up development environment (React + Vite)
- [ ] Implement responsive navigation
- [ ] Build homepage with hero section
- [ ] Build about page with biography
- [ ] Build portfolio grid with filtering
- [ ] Build portfolio case study template
- [ ] Implement basic SEO (meta tags, semantic HTML)

**Nice-to-Have**:

- [ ] Page transitions and animations
- [ ] Dark mode toggle
- [ ] Portfolio search functionality

**Deliverables**:

- Functional website on staging environment
- All core pages implemented
- Mobile responsive on all breakpoints

### Phase 4: Polish & Optimization (1-2 weeks)

**Must-Have**:

- [ ] Image optimization and lazy loading
- [ ] Performance audit and fixes
- [ ] Cross-browser testing (Chrome, Firefox, Safari)
- [ ] Mobile device testing
- [ ] Accessibility audit (WCAG AA compliance)
- [ ] SEO audit and optimization

**Nice-to-Have**:

- [ ] Advanced animations and micro-interactions
- [ ] Analytics integration (Google Analytics/Plausible)
- [ ] A/B testing setup
- [ ] Service worker for offline access

**Deliverables**:

- Performance report (Lighthouse scores)
- Accessibility audit report
- Browser compatibility matrix

### Phase 5: Launch & Post-Launch (1 week)

**Must-Have**:

- [ ] Deploy to production hosting
- [ ] Configure custom domain and SSL
- [ ] Submit sitemap to search engines
- [ ] Set up monitoring and error tracking
- [ ] Create backup strategy

**Nice-to-Have**:

- [ ] Set up CI/CD pipeline
- [ ] Configure CDN
- [ ] Social media launch announcement
- [ ] Create maintenance schedule

**Deliverables**:

- Live website
- Deployment documentation
- Maintenance plan

### Priority Matrix

**Must-Have (P0)**: Core functionality for launch

- Homepage, About, Portfolio pages
- Mobile responsive
- Basic SEO
- Performance optimization

**Nice-to-Have (P1)**: Enhancements post-launch

- Blog functionality
- Advanced animations
- Dark mode
- Analytics

**Future Enhancements (P2)**: Long-term improvements

- Multilingual support
- Interactive resume download
- Testimonials section
- Case study videos

---

## 6. Inspiration & References

### Primary Inspiration Sites (User-Selected)

These sites directly inspire the design and functionality of this project:

1. **[Theodorus Clarence](https://theodorusclarence.com/)** ⭐
   - **What to Adopt**:
     - Clean hero section with name, title, and description
     - Animated text on hero for attention (character-by-character reveal)
     - Elegant color tone (neutral base with strategic accent colors)
     - Excellent typography hierarchy
   - **Implementation Plan**:
     - Use Framer Motion for text animations
     - Implement gradient text effects on name/title
     - Focus on whitespace and breathing room
     - Inter or similar geometric sans-serif font

2. **[Jacky Efendi](https://jackyef.com/)** ⭐
   - **What to Adopt**:
     - Fun, playful color scheme (vibrant but not overwhelming)
     - Name and description prominently displayed
     - Approachable, friendly personality through design
   - **Implementation Plan**:
     - Use vibrant accent colors (purple, teal, or blue)
     - Playful hover interactions with color shifts
     - Micro-animations on interactive elements
     - Balance professionalism with personality

3. **[Bartosz Jarocki CV](https://cv.jarocki.me/)** ⭐
   - **What to Adopt**:
     - Command palette with `Cmd + J` keyboard shortcut
     - Quick navigation and actions via keyboard
     - Efficient, power-user focused interactions
   - **Implementation Plan**:
     - Use `cmdk` library for command palette
     - Implement `Cmd+K` and `Cmd+J` shortcuts
     - Include quick actions:
       - Navigation (Home, About, Projects)
       - Copy email to clipboard
       - Download resume
       - Toggle theme
       - Open social links

4. **[Faldi](https://faldi.xyz/)** ⭐
   - **What to Adopt**:
     - Clear personal branding statement ("Product Engineer & Mentor")
     - Well-structured portfolio cards with:
       - Title
       - Description
       - Image (if available)
       - Tech stack badges
       - Live website link (if available)
       - GitHub link (if available)
   - **Implementation Plan**:
     - Create consistent `ProjectCard` component
     - Use tech stack pills/badges for quick scanning
     - External link icons (Lucide React: ExternalLink, Github)
     - Responsive grid (3 columns → 2 → 1)
     - Optional project images with fallback

### Additional Example Websites

5. **[Brittany Chiang](https://brittanychiang.com/)**
   - Clean, minimal design with excellent typography
   - Smooth scroll animations and transitions
   - Well-organized portfolio with detailed project cards
   - **Key Takeaway**: Simplicity and attention to typography

6. **[Lee Robinson (Vercel VP)](https://leerob.io/)**
   - Exceptional blog with great content structure
   - Fast performance and excellent SEO
   - Clean, readable design focused on content
   - **Key Takeaway**: Content-first approach, performance matters

7. **[Josh Comeau](https://www.joshwcomeau.com/)**
   - Exceptional use of interactive elements and animations
   - Detailed blog posts with custom visualizations
   - Playful micro-interactions throughout
   - **Key Takeaway**: Interactive elements enhance engagement

### Design Trends for 2026

**Recommended Trends**:

1. **Glassmorphism & Frosted Glass Effects**
   - Subtle backdrop blur for cards and modals
   - Creates depth and modern aesthetic

2. **Bold Typography**
   - Large, expressive headings
   - Creative use of font weights and sizes

3. **Micro-interactions**
   - Subtle hover effects and animations
   - Feedback for user actions
   - Enhances perceived performance

4. **Dark Mode**
   - User preference detection
   - Smooth theme transitions
   - Reduced eye strain for users

5. **Asymmetric Layouts**
   - Breaking away from rigid grids
   - Creates visual interest
   - Maintains balance and harmony

**Trends to Avoid**:

- Overly complex animations that hurt performance
- Auto-playing videos without user control
- Excessive parallax scrolling (causes motion sickness)
- Splash screens or loading animations (adds friction)
- Generic stock photos (lacks authenticity)

### Design Resources

**Color Tools**:

- [Coolors.co](https://coolors.co/) - Color palette generator
- [Adobe Color](https://color.adobe.com/) - Color wheel and schemes
- [Contrast Checker](https://webaim.org/resources/contrastchecker/) - WCAG compliance

**Typography**:

- [Google Fonts](https://fonts.google.com/) - Free web fonts
- [Font Pair](https://fontpair.co/) - Font pairing suggestions
- [Type Scale](https://typescale.com/) - Visual type scale calculator

**Imagery**:

- [Unsplash](https://unsplash.com/) - Free high-quality photos
- [Shots.so](https://shots.so/) - Device mockup generator
- [Remove.bg](https://remove.bg/) - Background removal tool

**Icons**:

- [Heroicons](https://heroicons.com/) - Beautiful SVG icons
- [Lucide](https://lucide.dev/) - Icon toolkit
- [Font Awesome](https://fontawesome.com/) - Comprehensive icon library

---

## Implementation Requirements (EARS Format)

### Global Requirements

**UR-001**: The website shall be fully responsive across all device sizes (320px - 2560px)

**UR-002**: The website shall load the initial view in under 3 seconds on 3G connection

**UR-003**: The website shall achieve minimum 90 Lighthouse performance score

**UR-004**: The website shall meet WCAG 2.1 Level AA accessibility standards

**UR-005**: The website shall work on the latest two versions of Chrome, Firefox, Safari, and Edge

### State-Driven Requirements

**SD-001**: While viewing on mobile devices (< 768px), the navigation shall display as a hamburger menu

**SD-002**: While scrolling past the hero section, the header shall become sticky with background

**SD-003**: While in dark mode, the color scheme shall invert to light text on dark background

**SD-004**: While loading images, the system shall display skeleton placeholders

### Event-Driven Requirements

**ED-001**: When a user clicks a portfolio item, the system shall navigate to the case study page

**ED-002**: When a user hovers over a project card, the system shall display a subtle elevation effect

**ED-003**: When a page loads, the system shall animate content with fade-in transitions

### Optional Features

**OF-001**: Where a blog exists, the system shall support RSS feed subscription

**OF-002**: Where dark mode is implemented, the system shall remember user preference in localStorage

**OF-003**: Where portfolio filtering is implemented, the system shall update URL parameters for shareability

### Unwanted Behavior Requirements

**UB-001**: If an image fails to load, then the system shall display a fallback placeholder

**UB-002**: If JavaScript is disabled, then the website shall still display all content (progressive enhancement)

**UB-003**: If a 404 page is accessed, then the system shall display a helpful error page with navigation

---

## Success Metrics

**At Launch**:

- Website accessible via custom domain with SSL
- All core pages (Home, About, Portfolio) functional
- 6-10 portfolio projects with case studies
- Lighthouse performance score ≥ 90
- Lighthouse accessibility score ≥ 90
- Mobile-responsive on all breakpoints
- Contact information easily accessible (email, social links)

**Post-Launch (3 months)**:

- Average page load time < 2 seconds
- Bounce rate < 60%
- Average session duration > 2 minutes
- Positive engagement through social media and email
- Zero critical accessibility issues

**Long-Term (6 months)**:

- Ranking on first page for "[Your Name]" search
- 500+ unique visitors per month
- Portfolio showcased in job applications with positive feedback
- Blog (if implemented) with 10+ published articles

---

## Next Steps

1. **Review and customize** this roadmap based on your specific field and goals
2. **Gather content** - Start writing biography and collecting portfolio materials
3. **Choose tech stack** - Confirm React + Vite + TypeScript setup
4. **Create design mockups** - Use Figma to visualize the design
5. **Start Phase 1** - Begin with content preparation while design is in progress

---

**Document Version**: 2.1
**Last Updated**: 2026-01-07
**Owner**: Muhamad Eriansya (Ivan Putra Eriansya)
**Status**: Ready for Implementation
**Major Updates**:

- v2.0: Added comprehensive Code Structure & Technical Architecture section (Section 4)
- v2.1: Updated to use shadcn/ui + Tailwind CSS and TanStack Router (replacing React Router)
