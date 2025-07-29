# Code Standards

The following are code standards that a team can adopt. These code standards can change over
time as opinions, preferences and the overal development ecosystem changes.

## General

### TODO

- Git commits and messages
  - Review diff before committing
  - Review any AI generated code and understand what it's doing
- Linting and formatting setup in Editor
- Iterative development
- Testing standards
- If statement branching / early exiting
- Code review standards
  - Tools remove nitpicks (formatting, CI, PR templates)
  - Feedback
  - Self-review your PR before requesting review

### Git

- Commit strategy and messages (intent)
- Review diff before committing
- 

### Code Review

- Always self-review your PRs before requesting review

### Testing

- Always test your code

### AI

- Always review any AI generated code

### Techniques

- Flat if/else statements with early existing/guard statements to prevent nesting
- Truth tables

## TypeScript Projects

- Formatting
  - Use @ianvs/prettier-plugin-sort-imports and prettier-plugin-tailwindcss

## Databases

- Use PlanetScale. Their ability to scale on MySQL/Vitess and now PostgreSQL make it a no brainer. Their branching andDeploy Request features makes managing online schema changes easy.

# Standards to explore

- Vendoring vs Packages
