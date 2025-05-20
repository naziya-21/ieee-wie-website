# IEEE Women in Engineering (WIE) - VIT Chapter Website

A responsive, dark-themed website for the IEEE Women in Engineering Student Chapter at VIT University, built with React, TypeScript, and Tailwind CSS.

## Project Overview

This website serves as the official online presence for the IEEE WIE student chapter at VIT. It presents the chapter's mission, leadership team, events, and membership details while visually aligning with the IEEE WIE brand.

## Features

- 📱 **Fully Responsive Design**: Optimized for all screen sizes
- 🌙 **Dark Theme**: Elegant black background with purple/violet accents
- 🧩 **Component-Based Architecture**: Built with React and TypeScript
- 🎨 **Modern UI**: Designed with Tailwind CSS and shadcn/ui components
- 🔍 **SEO Friendly**: Includes meta tags and semantic HTML

## Pages/Sections

- **Home/Hero**: Overview of the chapter with key statistics
- **About**: Mission, vision, and history of the IEEE WIE VIT chapter
- **Team**: Leadership profiles with roles and contact details
- **Events**: Upcoming and past events with registration links
- **Membership**: Information on how to join with benefits
- **Contact**: Contact form and social media links

## Technologies Used

- React
- TypeScript
- Tailwind CSS
- Express (backend)
- shadcn/ui components
- React Query

## Getting Started

### Prerequisites

- Node.js 16+ installed
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/naziya-21/ieee-wie-website.git
cd ieee-wie-website
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5000`

## Project Structure

```
├── client/                  # Frontend code
│   ├── src/                 # React source files
│   │   ├── components/      # UI components
│   │   ├── hooks/           # Custom React hooks
│   │   ├── lib/             # Utility functions
│   │   ├── pages/           # Page components
│   │   └── types/           # TypeScript types
│   └── index.html           # HTML entry point
├── server/                  # Backend code
│   ├── index.ts             # Server entry point
│   └── routes.ts            # API routes
└── shared/                  # Shared code between client and server
    └── schema.ts            # Database schema
```

## Customization

You can customize the colors, content, and components to match your specific IEEE chapter's branding:

- Edit `tailwind.config.ts` to change theme colors
- Modify the content in component files to update text and images
- Add additional components as needed

## Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/my-new-feature`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- IEEE Women in Engineering for inspiration
- shadcn/ui for the component library
- All contributors and maintainers