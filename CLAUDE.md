# Project Name

Personal website to showcase project and portofolio

## Tech Stack

- Framework: React 19 + TypeScript
- Build Tool: Vite
- Styling: Tailwind CSS and shadcn/ui

## Preferred Patterns

### React

- Use functional components with TypeScript
- Prefer default exports over named exports
- Component files: PascalCase (ProjectCard.tsx)

### Styling

- Tailwind utility classes for all styling
- Use `className` helper for conditional classes
- Responsive: mobile-first approach
- Dark mode: use `dark:` variants

### Typescript

- Use TypeScript, so it should use .tsx instead of .js whenever applicable

### Testing Approach

- Always use case insensitive regex to assert text in testing, avoid hardcoded strings because they are case sensitive
- Whenever I change any implementation details, please update the corresponding tests to reflect those changes.

## Important Rules

- **NO** class component
- **PREFER** semantic HTML (header, nav, main, footer, section)
- **ALWAYS** add alt text to images for accessibility

## Development

```bash
# Install dependencies
bun install

# Run dev server
bun dev

# Build for production
bun run build

# Build preview
bun run preview

# linting all
bun run lint
```
