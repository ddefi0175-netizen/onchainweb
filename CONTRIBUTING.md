# Contributing to OnChainWeb

## Code Standards

- **TypeScript**: Strict mode enabled
- **Linting**: ESLint with modern rules (zero warnings policy)
- **Style**: EditorConfig for consistency
- **Package Manager**: npm (Node >= 18.0.0)

## Development Setup

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Type checking
npm run type-check

# Linting
npm run lint

# Full check before deploy
npm run check
```

## Deployment

```bash
# Dry run
npm run deploy:dry-run

# Production deploy
npm run deploy
```

## Stability Guidelines

1. **Pin Dependency Versions**: Always use exact versions in package.json
2. **Test Before Deploy**: Run `npm run check` to validate everything
3. **Type Safety**: Keep TypeScript strict mode enabled
4. **Linting**: Zero warnings policy - fix all lint issues
5. **Environment Variables**: Use .env and .dev.vars for sensitive data

## File Structure

```
onchainweb/
├── src/
│   ├── worker/     # Cloudflare Worker entry
│   ├── client/     # React client app
│   └── styles/     # CSS files
├── public/         # Static assets
├── dist/           # Build output (generated)
└── config files    # (tsconfig, vite.config, wrangler.json, etc.)
```
