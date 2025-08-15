# Code Standards

The following are code standards that a team can adopt. These code standards can change over
time as opinions, preferences and the overal development ecosystem changes.

## General

These are general standards that can be applied across languages and technologies.

### Editor Setup

- Formatting, linting, type checking done by editor

### Git

- Commit strategy and messages (intent)
- Review diff before committing
- Use a tool like [lazygit](https://github.com/jesseduffield/lazygit) which makes it easier to stage chunks
- GitHub Team plan with Branch Restrictions

### Technical Design Docs

TBD

### Code Review

- Always self-review your PRs before requesting review
- A note on giving and receiving feedback
- Remove nitpicks with tooling (format on save, CI, PR templates). Even reading this doc won't prevent some issues that tooling can remove completely

### Testing

- Always test your code
- Unit testing vs
- Regression testing

### AI

- Always review any AI generated code (and have an understanding of what the code's doing)
- [CodeRabbit?](https://www.coderabbit.ai/)

### Techniques

- Iterative development
- Flat if/else statements with early existing/guard statements to prevent nesting
- Truth tables

## TypeScript Projects

- Formatting
  - Use @ianvs/prettier-plugin-sort-imports and prettier-plugin-tailwindcss

## Databases

- Use PlanetScale. Their ability to scale on MySQL/Vitess and now PostgreSQL make it a no brainer. Their branching and Deploy Request features makes managing online schema changes easy.
- Add schema standards for naming tables, columns keys, etc.

## Tech Evaluation for Adoption

- Packages
- Third party services
- Langages

## Standards to explore

- Vendoring vs Packages
