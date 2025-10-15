# Contributing to Neurodivergent History Hub 🧠✨

**Thank you for your interest in contributing!** We're thrilled to have you here and excited to work with you. This project is built by and for the neurodivergent community, and we value contributions of all kinds—big or small!

## 🎯 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Coding Guidelines](#coding-guidelines)
- [Accessibility Requirements](#accessibility-requirements)
- [Submitting Changes](#submitting-changes)
- [Community & Support](#community--support)

## 📜 Code of Conduct

This project adheres to the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to conduct@hyperfocuszone.com

## 🤝 How Can I Contribute?

There are many ways to contribute to this project, regardless of your technical skill level:

### 🐛 Report Bugs
Found a bug? Let us know!
- Check if the issue already exists in our [issue tracker](https://github.com/yourusername/neurodivergent-history-hub/issues)
- If not, [create a new bug report](https://github.com/yourusername/neurodivergent-history-hub/issues/new?template=bug_report.md)
- Include as much detail as possible (screenshots, steps to reproduce, browser info)

### 💡 Suggest Features
Have an idea? We want to hear it!
- [Open a feature request](https://github.com/yourusername/neurodivergent-history-hub/issues/new?template=feature_request.md)
- Describe the feature and why it would be valuable
- If possible, suggest how it could be implemented

### ♿ Report Accessibility Issues
Accessibility is our priority!
- [Report accessibility problems](https://github.com/yourusername/neurodivergent-history-hub/issues/new?template=accessibility_issue.md)
- Include details about your assistive technology or accessibility needs
- Describe the barrier you encountered

### 📖 Improve Documentation
Documentation is crucial for accessibility!
- Fix typos or clarify confusing sections
- Add examples or tutorials
- Translate documentation into other languages
- Create video tutorials or visual guides

### 📚 Add Historical Content
Help us expand our knowledge base!
- Research and add neurodivergent historical figures
- Write accessible biographies and achievement summaries
- Fact-check existing content
- Add timeline entries for important events

### 💻 Write Code
Fix bugs, add features, or improve performance!
- Check out issues labeled [`good first issue`](https://github.com/yourusername/neurodivergent-history-hub/labels/good%20first%20issue)
- Look for [`help wanted`](https://github.com/yourusername/neurodivergent-history-hub/labels/help%20wanted) tags
- Improve accessibility features
- Optimize performance

### 🎨 Design Contributions
Make the project more beautiful and usable!
- Create icons, illustrations, or graphics
- Design new themes or color schemes
- Improve UI/UX
- Create promotional materials

### 🧪 Test & Provide Feedback
Your testing helps everyone!
- Test new features and report issues
- Try the app with different assistive technologies
- Provide user experience feedback
- Share your accessibility needs

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- A text editor or IDE (VS Code recommended)
- Git installed on your computer
- Basic knowledge of HTML, CSS, and JavaScript (for code contributions)

### Fork & Clone

1. **Fork the repository** by clicking the "Fork" button at the top right of this page

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/neurodivergent-history-hub.git
   cd neurodivergent-history-hub
   ```

3. **Add the upstream repository**
   ```bash
   git remote add upstream https://github.com/original-owner/neurodivergent-history-hub.git
   ```

4. **Create a new branch** for your work
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/bug-description
   ```

### Local Development

Simply open `index.html` in your browser, or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node.js (if you have http-server installed)
npx http-server

# Then visit http://localhost:8000
```

## 🔄 Development Workflow

### ADHD-Friendly Workflow

We recognize that contributors may have ADHD or other conditions. Here's a flexible workflow:

1. **Pick ONE issue** to focus on (avoid overwhelm!)
2. **Comment on the issue** to let others know you're working on it
3. **Work in short bursts** (Pomodoro technique: 25 min work, 5 min break)
4. **Commit frequently** with clear messages
5. **Ask for help** anytime—no question is too small
6. **Take breaks** when needed—your wellbeing comes first

### Making Changes

1. **Make your changes** in your feature branch
2. **Test thoroughly** - check in multiple browsers if possible
3. **Run accessibility checks** (see below)
4. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add: Brief description of your changes"
   ```

### Commit Message Guidelines

Use clear, descriptive commit messages:

- `Add: Description` - for new features
- `Fix: Description` - for bug fixes
- `Update: Description` - for updates to existing features
- `Remove: Description` - for removing code/features
- `Docs: Description` - for documentation changes
- `Style: Description` - for formatting/style changes
- `Test: Description` - for adding or updating tests
- `Accessibility: Description` - for accessibility improvements

**Examples:**
- ✅ `Add: Keyboard navigation for timeline section`
- ✅ `Fix: Screen reader not announcing profile cards`
- ✅ `Accessibility: Improve color contrast in dark mode`

## 📝 Coding Guidelines

### General Principles

- **Keep it simple** - Readable code is better than clever code
- **Comment your code** - Explain WHY, not just WHAT
- **Use semantic HTML** - Proper tags for proper meaning
- **Mobile-first** - Design for small screens, enhance for large
- **Progressive enhancement** - Core features work without JS

### HTML Guidelines

- Use semantic HTML5 elements (`<nav>`, `<article>`, `<section>`, etc.)
- Include proper ARIA labels and roles
- Use heading hierarchy correctly (h1 → h2 → h3)
- All images must have descriptive `alt` text
- Forms must have associated `<label>` elements

**Example:**
```html
<button 
  class="profile-card"
  aria-label="View profile of Albert Einstein"
  role="button"
  tabindex="0">
  <h3>Albert Einstein</h3>
  <p>Physicist and Revolutionary Thinker</p>
</button>
```

### CSS Guidelines

- Use CSS custom properties (variables) for consistency
- Follow BEM naming convention when appropriate
- Ensure minimum 4.5:1 color contrast ratio (WCAG AA)
- Support user font size preferences (use `rem` not `px`)
- Test with browser zoom up to 200%

**Example:**
```css
:root {
  --color-primary: #4A90E2;
  --color-text: #333333;
  --spacing-base: 1rem;
  --font-size-base: 1rem;
}

.profile-card {
  padding: var(--spacing-base);
  font-size: var(--font-size-base);
  color: var(--color-text);
}
```

### JavaScript Guidelines

- Use vanilla JavaScript (no framework dependencies)
- Use `const` and `let`, avoid `var`
- Write functions that do ONE thing well
- Handle errors gracefully with try/catch
- Save user preferences to localStorage
- Provide clear console messages for debugging

**Example:**
```javascript
// Save user preferences
function savePreferences(preferences) {
  try {
    localStorage.setItem('userPrefs', JSON.stringify(preferences));
    console.log('✅ Preferences saved successfully');
  } catch (error) {
    console.error('❌ Failed to save preferences:', error);
    showErrorMessage('Could not save your preferences');
  }
}
```

## ♿ Accessibility Requirements

**All contributions MUST meet these accessibility standards:**

### Mandatory Requirements

1. **Keyboard Navigation**
   - All interactive elements accessible via Tab key
   - Visible focus indicators
   - Logical tab order

2. **Screen Reader Support**
   - Proper ARIA labels
   - Alt text for images
   - Semantic HTML structure

3. **Color & Contrast**
   - Minimum 4.5:1 contrast ratio for text
   - Don't rely on color alone to convey information
   - Test with color blindness simulators

4. **Text & Typography**
   - Text must be resizable up to 200%
   - Line height of at least 1.5
   - Support for user font preferences

5. **Forms & Inputs**
   - Clear labels for all inputs
   - Error messages that are clear and helpful
   - Success confirmations

### Testing Accessibility

Before submitting, test your changes:

**Automated Testing:**
- [WAVE Browser Extension](https://wave.webaim.org/extension/)
- [axe DevTools](https://www.deque.com/axe/devtools/)
- Chrome Lighthouse (Accessibility audit)

**Manual Testing:**
- Navigate using only keyboard (Tab, Enter, Arrow keys)
- Test with a screen reader (NVDA, JAWS, VoiceOver)
- Zoom to 200% and verify layout
- Check color contrast with online tools

## 📤 Submitting Changes

### Before You Submit

✅ **Checklist:**
- [ ] Code follows the style guidelines
- [ ] Comments added to explain complex logic
- [ ] Accessibility requirements met
- [ ] Tested in multiple browsers
- [ ] Tested with keyboard navigation
- [ ] No console errors
- [ ] Commit messages are clear and descriptive

### Creating a Pull Request

1. **Push your changes** to your fork
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Open a Pull Request**
   - Go to the original repository on GitHub
   - Click "New Pull Request"
   - Select your fork and branch
   - Fill out the PR template completely

3. **PR Description Should Include:**
   - What changes you made and why
   - Related issue number (e.g., "Fixes #123")
   - Screenshots or videos (if UI changes)
   - Accessibility testing results
   - Any breaking changes

**Example PR Title:**
- ✅ `Add: Voice input support for search functionality`
- ✅ `Fix: Timeline not scrolling on mobile devices`
- ✅ `Accessibility: Improve focus indicators in dark mode`

### Review Process

1. **Maintainers will review** your PR within 3-7 days
2. **Address feedback** - we may request changes
3. **Once approved**, your PR will be merged! 🎉
4. **Celebrate** - you've just made history more accessible!

## 💬 Community & Support

### Need Help?

- **Discord** - [Join our community](https://discord.gg/your-invite)
- **GitHub Discussions** - [Ask questions](https://github.com/yourusername/neurodivergent-history-hub/discussions)
- **Email** - support@hyperfocuszone.com

### Response Time

We aim to respond to issues and PRs within **3-7 days**. If you need accommodations or have urgent accessibility concerns, please email us directly.

### Mentorship

New to open source? We offer mentorship!
- Comment on issues tagged `good first issue`
- Mention you're new and need guidance
- We'll pair you with an experienced contributor

## 🎉 Recognition

All contributors are recognized in our [CONTRIBUTORS.md](CONTRIBUTORS.md) file. Your contributions matter, no matter how small!

## 📚 Additional Resources

- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [WCAG 2.2 Guidelines](https://www.w3.org/WAI/WCAG22/quickref/)
- [Writing Accessible HTML](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)
- [Inclusive Design Principles](https://inclusivedesignprinciples.org/)

---

**Thank you for making history more accessible! 💜**

*Questions? Reach out anytime. We're here to help!*