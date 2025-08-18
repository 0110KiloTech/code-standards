# Code Standards

The following are code standards that a team can adopt. These code standards can change over
time as opinions, preferences and the overall development ecosystem changes.

## General

These are general standards that can be applied across languages and technologies.

### Editor Setup

- Ensure tooling allows for your team to use multiple IDEs and editors
- Your editor should be setup to follow your team's standards. This can included automatic linting and type checking, as well as, automatic formatting on save. This will prevent unnecessary commits to fix these issues when enforced by CI.

### Git

- Adopt a standard for commits and commit messages. Consider [Conventional Commits](https://www.conventionalcommits.org/) or [Seven Rules method](https://cbea.ms/git-commit/). Additional resources: [git docs](https://git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project), [another resource](https://wiki.openstack.org/wiki/GitCommitMessages), [another resource](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html), and [another resource](https://drewdeponte.com/blog/how-we-should-be-using-git/)
- Review the diff before committing and break commits up into smaller units by staging chunks
- Use a tool like [lazygit](https://github.com/jesseduffield/lazygit) which makes it easier to stage chunks
- Determine if your team wants to squash and merge, rebase and merge or use standard merge commits

### Code Review

- Always self-review your PRs before requesting review
- Add a [PR template](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository) and adopt a consistent convention for titles (e.g. ISSUE-1234 Issue title from issue tracker)
- Remove nitpicks with tooling (format on save, CI, PR templates), as well as, enforce any code standards
- Give feedback kindly and directly, focusing on the code and explaining the "why." Receive feedback with openness, assuming positive intent and remembering it's about improving the work, not the person

### Testing

- Always test your code before PR review and after deployment to production

### AI

- Utilize AI tools as much as possible to offload tedious, tiring and sometimes difficult work
- Utilize AI tools to allow you to focus more on the product, your users and more complicated problems
- Until AI tools advance further (which may be sooner than later), treat them like a junior engineer that is very smart, knowledgable, but doesn't necessarily have the context or tribal knowledge to work unsupervised
- We using an AI agent to write code, keep in mind that it's much harder to grasp what code is doing when you haven't written any of the logic. You may find that it gets you 80% of the way there and then leave you hanging
- Always review any AI generated code, have an understanding of what the code is doing, and try to make it your own

## TypeScript Projects

- Formatting / Linting
  - Use [@ianvs/prettier-plugin-sort-imports](https://github.com/IanVS/prettier-plugin-sort-imports) and prettier-plugin-tailwindcss
- Require semicolons, trailing commas, curly braces for if statements

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
