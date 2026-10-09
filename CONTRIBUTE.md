# Contributing

Thank you for your interest in improving Cowork vs Copilot Advisor. Contributions
that make the guidance clearer, more accurate, and easier to use are welcome.

## Before You Start

- Search existing issues and pull requests to avoid duplicating work.
- Open an issue before making a large or behavior-changing contribution.
- Keep changes focused on a single topic.
- Do not include confidential information, customer data, credentials, or
  proprietary content.

## Ways to Contribute

You can help by:

- Correcting inaccurate or outdated guidance
- Improving the decision model, examples, or guardrails
- Clarifying installation and usage instructions
- Fixing typos, broken links, or formatting
- Reporting bugs or proposing enhancements

## Development Workflow

1. Fork the repository.
2. Create a branch from the default branch:

   ```text
   git checkout -b type/short-description
   ```

   Common branch prefixes include `docs/`, `fix/`, and `feature/`.

3. Make your changes.
4. Review and validate the affected files.
5. Commit with a clear, concise message.
6. Push your branch and open a pull request.

## Repository Structure

- `cowork-vs-copilot-advisor/SKILL.md` contains the skill definition, decision
  logic, output format, and guardrails.
- `README.md` describes the project and its capabilities.
- `INSTALL.md` explains how to package and install the skill.

## Contribution Guidelines

- Preserve the cost-first principle: recommend Microsoft 365 Copilot when both
  products can complete the task adequately.
- Do not invent pricing, product capabilities, licensing terms, or consumption
  estimates.
- Clearly label assumptions and uncertainty.
- Keep recommendations concise, practical, and decision-oriented.
- Use examples that do not contain personal, confidential, or sensitive data.
- Update related documentation when behavior or installation steps change.
- Follow the existing Markdown style and terminology.

## Validation

This repository does not currently include an automated test suite. Before
opening a pull request:

- Preview changed Markdown files and check their formatting.
- Verify that links resolve correctly.
- Check spelling, headings, lists, tables, and code blocks.
- Confirm that changes to `SKILL.md` remain internally consistent.
- Test representative prompts when changing decision logic or output behavior.
- If packaging is affected, follow `INSTALL.md` and verify the archive structure.

In your pull request, describe the validation you performed.

## Reporting Issues

When reporting a problem, include:

- A clear title and description
- Steps or a sample prompt that reproduces the issue
- The expected and actual behavior
- Relevant screenshots or output with sensitive information removed
- Any suggested solution, if you have one

## Pull Requests

Pull requests should:

- Explain what changed and why
- Reference related issues
- Avoid unrelated formatting or cleanup
- Include updated documentation where needed
- Be ready for review and respond to requested changes

By submitting a contribution, you agree that it may be distributed under the
repository's MIT License.