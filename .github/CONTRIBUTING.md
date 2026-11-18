# Contributing to Graupl

Read these guidelines before contributing code, documentation, bug reports, or feature requests.

## Write for the people who use and maintain this project

Graupl is part of Accessible Ecosystem and helps people who may use the web differently than we do. Contributions should reflect the same care we put into making the web more accessible and friendly for everyone.

Accessibility also includes the people reading our code and documentation. Write plainly so someone just entering the field can follow your work, while giving experienced developers the detail they need to understand and maintain it.

- Use descriptive names, clear steps, and straightforward conditions. Avoid clever shortcuts that make the code harder to understand.
- Follow the project's existing structure and conventions. Introduce shared code when it makes the behavior easier to follow, rather than simply reducing the number of lines.
- Explain decisions and behavior that are not obvious. Keep comments useful, and update affected documentation when behavior changes.
- Keep contributions focused on the problem they address. Avoid unrelated cleanup or refactoring.
- Preserve existing behavior unless the contribution intentionally changes it. Consider keyboard interactions, focus, events, and compatibility.
- Use the relevant accessibility standards and ARIA Authoring Practices Guide patterns when changing accessibility behavior. Check HTML examples and generated markup for validity.
- Test the behavior your contribution affects. Passing automated checks alone does not establish that an interaction is accessible.

By submitting any contribution, you take responsibility for its contents, whether you wrote it yourself or used assistance. Submit work you understand, have reviewed, and can explain.

Read the [project instructions](../AGENTS.md) and [accessibility policy](ACCESSIBILITY.md) before contributing. AI-assisted contributions must also follow the [AI contribution policy](AI_CONTRIBUTIONS.md).

## Where to contribute

We use GitHub to host code, track bugs and feature requests, and review pull requests. Use GitHub issues and pull requests so project discussions and decisions are available to contributors.

## Submit a pull request

All code changes happen through pull requests.

1. Fork the repository and create your branch from `1.x`.
2. Make your changes and update any affected documentation.
3. Add or update tests that demonstrate the intended behavior where the change needs test coverage.
4. Run the relevant tests and code checks described below. Verify the affected behavior yourself.
5. Open your pull request and link any relevant issues. Describe the change, how you verified it, and any remaining limitations.

## Contribution license

Contributions must use the same license as the project, [GNU General Public License v3.0 or later](../LICENSE), identified as `GPL-3.0-or-later` in `package.json`.

## Report a bug

Report bugs by [opening a GitHub issue](https://github.com/Graupl/icons/issues/new).

Include the following in your bug report:

- A summary of the problem.
- Steps to reproduce it, with a small code example if possible.
- What you expected to happen.
- What actually happened.
- Any relevant background, such as your browser, package version, and anything you have already tried.

## Set up and check your changes

Use Node.js 24, which is also used by the project workflows. Run `npm install` to install the development tools.

Run commands from the repository root. Sass source lives in `src/scss/`, and public Sass entry points live in `scss/`.

Run `npm run stylelint` and `npm run prettier -- --check` to check the source. Run `npm run build` to regenerate the CSS and source maps in `dist/css/`. Review generated changes along with source changes.

Use `npm pack --dry-run` to check which files npm will publish.

## Commit guidelines

Write commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). For example:

```text
fix: cancel pending callbacks when disposing a component
```

The format is:

> \<type>[optional scope]: \<description>
>
> [optional body]
>
> [optional footer(s)]

See the specification for commit types, optional scopes, and how to describe breaking changes.

Commit messages must follow this format before a contribution can be merged.

## References

This document was adapted from the open-source contribution guidelines for [Facebook's Draft](https://github.com/facebook/draft-js/blob/a9316a723f9e918afde44dea68b5f9f39b7d9b00/CONTRIBUTING.md)

## Attribution

This document is based on [Accessible Ecosystem Core](https://github.com/Accessible-Ecosystem/core), adapted from its [corresponding document](https://github.com/Accessible-Ecosystem/core/blob/1.x/.github/CONTRIBUTING.md).
