# Content Validation Tool

A React TypeScript application for validating content from PDF to PDF and Word to PDF conversions.

## Project Structure

```
src/
├── components/          # Reusable components
│   ├── Button.tsx
│   ├── Input.tsx
│   ├── Card.tsx
│   └── Header.tsx
├── pages/              # Page components
│   ├── Login.tsx
│   └── Dashboard.tsx
├── styles/             # Stylesheet files
│   ├── index.css       # Global styles
│   ├── App.css
│   ├── pages/          # Page-specific styles
│   │   ├── Login.css
│   │   └── Dashboard.css
│   └── components/     # Component-specific styles
│       ├── Button.css
│       ├── Input.css
│       ├── Card.css
│       └── Header.css
├── App.tsx             # Main app component with routing
└── index.tsx           # React entry point
```

## Features

- **React 18** with TypeScript for type-safe development
- **React Router v6** for client-side routing
- **Reusable Components**: Button, Input, Card, Header
- **Login Page**: Authentication interface with form validation
- **Dashboard**: Main application interface with validation task management
- **Responsive Design**: Mobile-friendly CSS with media queries
- **Modern UI**: Material Design-inspired styling with CSS variables

## Prerequisites

- Node.js 16+ 
- npm or yarn package manager

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd content-validation-tool-QA
```

2. Install dependencies:
```bash
npm install
```

## Development

Start the development server:

```bash
npm start
```

The application will open at `http://localhost:3000`

## Building

Create an optimized production build:

```bash
npm run build
```

## Available Scripts

- `npm start` - Runs the development server
- `npm build` - Creates a production build
- `npm test` - Runs tests
- `npm eject` - Ejects from Create React App (not reversible)

## Component Guide

### Button
```tsx
<Button variant="primary" size="medium" fullWidth>
  Click me
</Button>
```

**Props:**
- `variant`: 'primary' | 'secondary' | 'tertiary' | 'danger'
- `size`: 'small' | 'medium' | 'large'
- `fullWidth`: boolean
- `disabled`: boolean

### Input
```tsx
<Input
  type="email"
  name="email"
  label="Email Address"
  placeholder="Enter email"
  error="Error message"
  helperText="Helper text"
/>
```

### Card
```tsx
<Card variant="outlined">
  Content here
</Card>
```

**Props:**
- `variant`: 'outlined' | 'elevated' | 'filled'

## Authentication

Currently, the authentication system is a placeholder. To implement:

1. Update the `isAuthenticated` state in `App.tsx`
2. Implement login logic in `Login.tsx`
3. Add authentication service/hooks
4. Implement token storage and verification

## Styling

The application uses CSS variables for theming. Edit `:root` in `src/styles/index.css` to customize colors and styling.

## Next Steps

- [ ] Implement authentication system
- [ ] Create API service layer
- [ ] Add validation file upload functionality
- [ ] Implement comparison logic
- [ ] Add report generation
- [ ] Create settings/admin pages
- [ ] Add unit and integration tests
- [ ] Setup state management (Redux/Zustand)
- [ ] Add error boundary components
- [ ] Implement logging

## Contributing

Follow the existing code structure and styling conventions. Create feature branches for new work.

## License

[Add your license here]
