# Code Standards

The following are code standards that a team can adopt. These code standards can change over
time as opinions, preferences and the overall development ecosystem changes.

## General

These are general standards that can be applied across languages and technologies.

### Editor Setup

- Ensure tooling allows for your team to use multiple IDEs and editors
- Your editor should be setup to follow your team's standards. This can included automatic linting and type checking, as well as, automatic formatting on save. This will prevent unnecessary commits to fix these issues when enforced by CI.

### Git

- Commit strategy and messages (intent)
- Review diff before committing
- Use a tool like [lazygit](https://github.com/jesseduffield/lazygit) which makes it easier to stage chunks
- GitHub Team plan with Branch Restrictions

### Code Review

- Always self-review your PRs before requesting review
- A note on giving and receiving feedback
- Remove nitpicks with tooling (format on save, CI, PR templates). Even reading this doc won't prevent some issues that tooling can remove completely

### Testing

- Always test your code before PR review and after deployment to production

### AI

- Always review any AI generated code (and have an understanding of what the code's doing)

## TypeScript Projects

- Formatting
  - Use @ianvs/prettier-plugin-sort-imports and prettier-plugin-tailwindcss
- ESLint
- Semicolons, trailing commas, curly for if statements

## Infrastructure

### Databases

- Use PlanetScale. Their ability to scale on MySQL/Vitess and now PostgreSQL make it a no brainer. Their branching and Deploy Request features makes managing online schema changes easy.

## Drafts

### General > Testing

- Unit Testing
- Integration Testing
- Smoke & Regression Testing
- End-to-end Testing

### General > CI/CD

- Setup a Continuous Integration environment (e.g. GitHub Actions) that will build, lint, test on every commit and merged PR

### General > AI

- Ensure your project has sufficient AI instruction files so AI tools can understand the codebase and standards to follow
- Utilize AI Code Reviews ([CodeRabbit](https://www.coderabbit.ai/))

### General > Database Schema Design

- Add schema standards for naming tables, columns keys, etc.

## TODO

- Tech Evaluation for Adoption in project or among team
- Technical Design Docs
- Techniques
  - Iterative development
  - Flat if/else statements with early existing/guard statements to prevent nesting
  - Truth tables
- Infrastructure as Code
- Immutable Infrastructure
- When to vendor packages
