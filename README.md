# Shared Integrations Monorepo

A monorepo containing reusable integration packages for Stripe, SendGrid, and Supabase across your projects.

## Packages

- `packages/stripe` - Stripe payment integration
- `packages/sendgrid` - SendGrid email integration  
- `packages/supabase` - Supabase database integration
- `packages/scheduler` - Task scheduler for Vercel, Railway, GitHub Actions, and Expo

## Installation

```bash
yarn install
```

## Building

```bash
yarn build
```

## Structure

Each package is self-contained with its own TypeScript configuration, dependencies, and source code. This makes it easy to extract individual packages into standalone npm packages later.

## Usage

Refer to individual package READMEs for usage instructions and examples.

## Adding to Projects

You can reference these packages locally during development:

```json
{
  "dependencies": {
    "@shared-integrations/stripe": "file:../shared-integrations/packages/stripe",
    "@shared-integrations/sendgrid": "file:../shared-integrations/packages/sendgrid",
    "@shared-integrations/supabase": "file:../shared-integrations/packages/supabase"
  }
}
```

Or publish to npm for easier cross-project reuse.
