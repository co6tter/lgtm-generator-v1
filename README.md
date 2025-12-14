# lgtm-generator-v1

## Overview

A web application for generating customizable LGTM (Looks Good To Me) images. Create personalized LGTM images with custom text, colors, templates, and text positioning for use in code reviews, pull requests, and team communications.

Features:
- Real-time canvas preview
- Multiple template options
- Customizable text color and background color
- Adjustable font size and text position
- Undo/Redo functionality
- Download images as PNG
- Share via Web Share API
- Copy shareable links with configuration
- Automatic local storage of settings
- History page to view previously generated images

## Tech Stack

- **Framework**: Next.js 15.5.6 with Turbopack
- **UI Library**: React 19.1.0
- **Language**: TypeScript 5
- **Styling**: Tailwind CSS 4
- **State Management**: Zustand 5.0.8
- **Icons**: Lucide React
- **Testing**: Vitest with Testing Library
- **Linting**: ESLint
- **Formatting**: Prettier with Tailwind CSS plugin

## Setup

1. Install dependencies:
```bash
npm install
```

2. Run the development server:
```bash
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Usage

### Basic Workflow
1. Enter your desired text (up to 50 characters)
2. Select a template from the available options
3. Adjust font size using the selector
4. Choose text position (top, middle, or bottom)
5. Customize text and background colors
6. Preview the generated image in real-time
7. Download the image or share it

### Available Commands
- `npm run dev` - Start development server with Turbopack
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier
- `npm test` - Run tests with Vitest
- `npm run test:ui` - Run tests with UI
- `npm run test:coverage` - Generate test coverage report

### Features
- **Undo/Redo**: Use Ctrl+Z / Ctrl+Y or the UI buttons
- **Auto-save**: All changes are automatically saved to local storage
- **Copy Link**: Generate a shareable URL with your configuration
- **Share**: Use the native share functionality (on supported devices)
- **History**: View previously generated LGTM images on the `/history` page

## Directory Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── history/           # History page
│   ├── page.tsx           # Home page
│   └── layout.tsx         # Root layout
├── components/            # React components
│   ├── actions/           # Action buttons (Download, Share, etc.)
│   ├── common/            # Reusable UI components
│   ├── editor/            # Editor-specific components
│   ├── layout/            # Layout components
│   └── pages/             # Page-level components
├── constants/             # Application constants
│   ├── colors.ts          # Color presets
│   ├── defaults.ts        # Default configuration
│   └── templates.ts       # Template definitions
├── lib/                   # Utility libraries
│   ├── canvas/            # Canvas rendering logic
│   ├── hooks/             # Custom React hooks
│   ├── storage/           # Local storage utilities
│   └── utils/             # General utilities
├── store/                 # Zustand state management
│   ├── editorStore.ts     # Editor state
│   └── uiStore.ts         # UI state
└── types/                 # TypeScript type definitions
```

## License

This repository is for personal/private use only.
