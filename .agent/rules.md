# Agent Rules for idlhy0218.github.io

## 🚨 CRITICAL RULE - NEVER VIOLATE THIS

### **NEVER Change File Paths in HTML Code**

**This is the most important rule. When editing ANY HTML file in this project:**

- **DO NOT** modify any file paths that reference GitHub repository structure
- **DO NOT** change relative paths like `../page building/`, `./blog/`, `../images/`, etc.
- **DO NOT** "fix" or "optimize" paths that look redundant (e.g., `../page building/blog/` is intentional)
- **DO NOT** convert relative paths to absolute paths or vice versa
- **DO NOT** reorganize folder structure without explicit user permission

**Examples of paths you must NEVER change:**
```html
<!-- NEVER change these -->
<link href="../page building/styles.css" rel="stylesheet">
<img src="../images/logo.png">
<a href="./blog/statslab/post.html">
<script src="../page building/blog/gallery/script.js"></script>
```

**Why this matters:** GitHub Pages has a specific deployment structure. Changing paths will break the live website even if it works locally.

---

## General Development Rules

### Code Modification Guidelines

1. **Ask Before Major Changes**
   - Always ask before refactoring large sections of code
   - Confirm before deleting files or moving them
   - Get approval before changing project structure

2. **Preserve Existing Patterns**
   - Follow the existing code style in the file you're editing
   - Don't introduce new frameworks or libraries without permission
   - Keep the same naming conventions used in the project

3. **Test Before Committing**
   - Verify changes don't break existing functionality
   - Check that all links still work
   - Ensure responsive design isn't broken

### File Editing Best Practices

1. **Keep Backups**
   - Don't delete old code immediately
   - Comment out instead of deleting when unsure
   - Keep version history in mind

2. **Document Changes**
   - Add comments explaining non-obvious changes
   - Update README if you change project structure
   - Note breaking changes clearly

### Common Mistakes to Avoid

❌ **DON'T:**
- Change file paths in HTML/CSS/JS files
- Edit generated files instead of source files
- Delete files without checking references
- Introduce breaking changes without warning
- Mix tabs and spaces inconsistently
- Commit commented-out code to production
- Use hardcoded values instead of variables
- Ignore existing code patterns

✅ **DO:**
- Preserve all existing file paths
- Follow the project's existing code style
- Ask before making structural changes
- Test changes thoroughly
- Use meaningful variable names
- Keep code DRY (Don't Repeat Yourself)
- Write clear commit messages
- Check for console errors

---

## Project-Specific Rules

### Blog Management

1. **Date Consistency**
   - Dates in `.qmd` files must match dates in `blog.html`
   - Use format: `"Month DD, YYYY"` (e.g., "Nov 30, 2025")
   - Update both locations when changing dates

2. **Blog Configuration**
   - All posts must be registered in `blog.html` blogConfig
   - Maintain alphabetical or chronological order
   - Include all required fields: id, title, date, description, file

3. **File Organization**
   - Stats Lab posts: `page building/blog/statslab/`
   - Study Notes: `page building/blog/studynotes/`
   - Gallery images: `page building/blog/gallery/`

### Design Consistency

1. **Navigation**
   - Keep nav items: About, Publications, Teaching, Blog, CV, Contact
   - Maintain mobile menu toggle functionality
   - Preserve logo and site title

2. **Styling**
   - Use existing CSS variables (`:root` definitions)
   - Maintain Financial Times-inspired theme
   - Keep Inter font family
   - Preserve responsive breakpoints

3. **JavaScript**
   - Use ES6+ syntax consistently
   - Maintain event-driven architecture
   - Keep tab-based interface structure

---

## Quality Checklist

Before finalizing any changes:

- [ ] All file paths remain unchanged
- [ ] No broken links or 404 errors
- [ ] Dates are consistent across files
- [ ] Code follows existing style
- [ ] Responsive design works on mobile
- [ ] No console errors in browser
- [ ] Changes are tested locally
- [ ] Documentation is updated if needed

---

## When in Doubt

**If you're unsure whether to make a change:**
1. **ASK THE USER FIRST**
2. Show them what you plan to change
3. Explain why you think it needs changing
4. Wait for confirmation

**Especially ask before:**
- Changing any file paths
- Deleting any files
- Restructuring folders
- Modifying core functionality
- Introducing new dependencies
- Making breaking changes

---

**Last Updated:** 2026-02-16  
**Project Owner:** Heeyoung Lee  
**Repository:** idlhy0218.github.io
