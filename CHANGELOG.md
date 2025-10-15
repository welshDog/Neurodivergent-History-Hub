# Changelog

All notable changes to the Neurodivergent History Hub project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned
- Mobile app version (iOS and Android)
- Multi-language support (Spanish, French, German)
- Advanced search with filters
- User authentication and profiles
- API for third-party integrations
- Audio descriptions for all visual content
- Export feature for personal learning notes

## [1.0.0] - 2025-10-15

### Added
- Initial public release of Neurodivergent History Hub
- Full accessibility control panel with font, theme, and text size options
- Four color themes: Light, Dark, High Contrast, and Neurodivergent-Friendly
- Dyslexia-friendly font option
- Interactive timeline with filterable historical events
- Notable figures section with detailed profile cards
- Profile cards for Albert Einstein, Temple Grandin, Richard Branson, and Frida Kahlo
- Community stories section for user contributions
- Achievement system with gamification badges
- Keyboard navigation throughout entire application
- Screen reader support with proper ARIA labels
- Distraction-free reading mode
- LocalStorage for persistent user preferences
- Responsive mobile-first design
- Semantic HTML5 structure for accessibility
- WCAG 2.2 Level AA compliance (targeting AAA)

### Documentation
- Comprehensive README with quick start guide
- Code of Conduct based on Contributor Covenant
- Detailed CONTRIBUTING guide with accessibility requirements
- MIT License for open-source usage
- Accessibility statement
- Project roadmap

### Infrastructure
- GitHub repository setup
- Issue templates (Bug Report, Feature Request, Accessibility Issue)
- Pull request template
- .gitignore for web development
- GitHub Actions workflow (future implementation)

## [0.5.0] - 2025-10-10

### Added
- Beta release for community testing
- Core timeline functionality
- Basic profile card system
- Accessibility panel prototype
- Theme switching capability

### Fixed
- Focus indicator visibility in dark mode
- Mobile navigation menu overflow
- Text scaling issues at 200% zoom
- Tab order for keyboard navigation

## [0.3.0] - 2025-10-01

### Added
- Alpha release for internal testing
- Initial HTML structure
- CSS styling system with custom properties
- JavaScript for theme switching
- LocalStorage implementation

### Changed
- Restructured navigation for better accessibility
- Improved color contrast ratios
- Updated heading hierarchy for screen readers

## [0.1.0] - 2025-09-15

### Added
- Project initialization
- Basic file structure
- Design system planning
- Accessibility research documentation

---

## Version Format

We follow [Semantic Versioning](https://semver.org/):
- **MAJOR** version (X.0.0): Incompatible changes or major redesigns
- **MINOR** version (0.X.0): New features, backward-compatible
- **PATCH** version (0.0.X): Bug fixes and minor improvements

## Change Categories

- **Added** - New features or functionality
- **Changed** - Changes to existing functionality
- **Deprecated** - Features that will be removed in future versions
- **Removed** - Features that have been removed
- **Fixed** - Bug fixes
- **Security** - Security vulnerability fixes
- **Accessibility** - Accessibility improvements or fixes

## How to Contribute to Changelog

When submitting a Pull Request, please add your changes to the `[Unreleased]` section:

1. Use the appropriate category (Added, Changed, Fixed, etc.)
2. Write in past tense ("Added feature" not "Add feature")
3. Be specific and concise
4. Link to related issues when applicable

**Example:**
```markdown
### Added
- Voice input support for search functionality [#42]
- Spanish language translation for timeline events [#56]

### Fixed
- Screen reader not announcing achievement unlocks [#38]
- Timeline scrolling on iOS Safari [#51]
```

---

For more information about contributing, see [CONTRIBUTING.md](CONTRIBUTING.md)