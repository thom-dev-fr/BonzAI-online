# AGENTS.md - BonzAI Online Repository Guide

This document provides guidelines for AI coding agents working in the BonzAI-online repository.

## Repository Overview

This is a static website repository for the BonzAI mobile app, hosted on GitHub Pages using Jekyll. The site contains:
- Legal documentation (privacy policy, terms of use) in English and French
- OAuth callback page for app authentication
- Apple App Site Association file for universal links

## Repository Structure

```
/
├── _config.yml                    # Jekyll configuration
├── index.md                       # Homepage
├── privacy-policy.md             # Privacy policy (English)
├── privacy-policy-fr.md          # Privacy policy (French)
├── terms.md                      # Terms of use (English)
├── terms-fr.md                   # Terms of use (French)
├── callback.html                 # OAuth callback redirect page
└── .well-known/
    └── apple-app-site-association # iOS universal links config
```

## Build/Test Commands

### Local Development

```bash
# Install Jekyll (if not already installed)
gem install bundler jekyll

# Serve locally (if Gemfile exists)
bundle exec jekyll serve

# Or use GitHub Pages gem
jekyll serve
```

### Testing

```bash
# Validate HTML files
# Open callback.html in a browser to test

# Check markdown rendering
# Preview .md files in any markdown viewer or GitHub

# Validate links manually
# Ensure all internal links in index.md work
```

### Deployment

- Deployment is automatic via GitHub Pages
- Push to `main` branch triggers auto-deployment
- Site URL: https://[username].github.io/BonzAI-online/

## Code Style Guidelines

### Markdown Files

**Formatting:**
- Use ATX-style headers (`#` prefix)
- Leave blank line before and after headers
- Use `-` for unordered lists
- Indent nested lists with 2 spaces
- Use `---` for horizontal rules
- Keep line length reasonable (80-100 chars when practical)

**Structure:**
- Start with H1 title (`#`)
- Use H2 (`##`) for main sections
- Use H3 (`###`) for subsections
- Maintain consistent header hierarchy

**Links:**
- Use relative paths for internal links: `[text](page.md)`
- Use descriptive link text (avoid "click here")

**Language-Specific Files:**
- English: `filename.md`
- French: `filename-fr.md`
- Maintain parallel structure between language versions

### HTML Files

**Style:**
- Use proper HTML5 DOCTYPE
- Include charset meta tag: `<meta charset="utf-8" />`
- Self-closing tags should use XHTML style: `<meta />`
- Use double quotes for attributes
- Indent with 2 spaces
- Include descriptive title tags

**JavaScript:**
- Use modern ES6+ syntax
- Prefer `const` over `let`, avoid `var`
- Use descriptive variable names (camelCase)
- Add comments for complex logic
- Keep inline scripts minimal and focused

### YAML Files

**Jekyll Configuration:**
- Use lowercase keys
- Quote strings only when necessary
- Use arrays with bracket notation: `[".well-known"]`
- Keep configuration minimal

## Content Guidelines

### Legal Documents

**Privacy Policy & Terms:**
- Maintain professional, clear language
- Use numbered or bulleted sections for clarity
- Keep English and French versions in sync
- Update copyright year when making changes
- Review changes carefully - legal documents require accuracy

**Structure:**
- Start with document title as H1
- Break into logical sections with H2/H3
- Use lists for rights, obligations, or processes
- Include effective date if applicable
- Add copyright footer: `© YYYY - BonzAI - Thomas LECONTE`

### Bilingual Content

**Consistency:**
- When updating English content, update French simultaneously
- Maintain parallel structure and equivalent information
- Keep formatting consistent between languages
- Use proper French characters and accents

**Translation:**
- Ensure translations are accurate and natural
- Legal terms should be properly translated (not literal)
- Maintain the same tone and formality level

## Git Workflow

### Commit Messages

Follow conventional commit format:

```
<type>: <description>

[optional body]
```

**Types:**
- `feat`: New content or functionality
- `fix`: Corrections to existing content
- `docs`: Documentation changes
- `style`: Formatting changes (no content change)
- `refactor`: Restructuring content

**Examples:**
```
feat: adding public page for oauth redirection
fix: correct privacy policy contact email
docs: update terms with new policy details
style: improve markdown formatting in index
```

### Commit Guidelines

- Use lowercase for commit message subjects
- Don't end subject with period
- Keep subject under 72 characters
- Write in imperative mood ("add" not "added")
- Reference issues if applicable: `fix: correct link (#123)`

## Common Tasks

### Adding a New Page

1. Create markdown file: `new-page.md`
2. Add French version: `new-page-fr.md`
3. Link from `index.md` in both language sections
4. Test links locally before committing

### Updating Legal Documents

1. Update English version first
2. Update French version for consistency
3. Review all changes carefully
4. Consider adding effective date to document
5. Commit with descriptive message

### Modifying OAuth Callback

1. Edit `callback.html`
2. Test URL parameter handling
3. Verify deep link scheme: `bonzai://callback`
4. Test in browser with sample parameters

## Best Practices

### Content Quality

- Proofread all content changes
- Verify links work correctly
- Check spelling and grammar
- Ensure consistent formatting
- Test HTML files in browser

### Repository Maintenance

- Keep commits atomic and focused
- Write clear commit messages
- Don't commit sensitive data
- Maintain clean git history
- Update copyright year annually

### Accessibility

- Use semantic HTML
- Provide descriptive link text
- Ensure proper heading hierarchy
- Keep content readable and clear

## Resources

- Jekyll Documentation: https://jekyllrb.com/docs/
- GitHub Pages: https://pages.github.com/
- Markdown Guide: https://www.markdownguide.org/
- HTML5 Spec: https://html.spec.whatwg.org/

---

**Note:** This is a minimal static site repository. There are no tests, linters, or build tools beyond Jekyll's built-in processing. Changes are deployed automatically when pushed to the main branch.
