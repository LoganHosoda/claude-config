# /new-design Command

Generate multiple unique design variations for website components using parallel sub-agents.

## Usage
```
/new-design "design requirements and component type"
```

## Examples
```
/new-design "modern navbar with search functionality and user dropdown"
/new-design "hero section for SaaS landing page with call-to-action"
/new-design "responsive footer with social links and newsletter signup"
/new-design "pricing table with three tiers and feature comparison"
/new-design "contact form with validation and modern styling"
```

## Process
1. Analyze existing project structure and design patterns
2. Create `/designs/{component-type}/` directory if it doesn't exist
3. Launch 3 parallel sub-agents to generate unique design variations
4. Each agent creates a complete HTML file with embedded CSS
5. Consider responsive design, accessibility, and modern web standards
6. Generate dynamic file names with timestamps for organization

## Output
Three distinct HTML files in `/designs/{component-type}/{timestamp}_variation_{1,2,3}.html`

Each file contains:
- Complete HTML structure
- Embedded CSS with modern styling approaches
- Responsive design considerations
- Accessibility features
- Comments explaining design decisions
- Documentation links for techniques used

## Design Variations Focus
- **Variation 1**: Modern/minimalist approach
- **Variation 2**: Bold/creative approach  
- **Variation 3**: Classic/professional approach

## File Structure Example
```
/designs/
  navbar/
    20250716_143052_variation_1.html
    20250716_143052_variation_2.html
    20250716_143052_variation_3.html
  hero-section/
    20250716_145123_variation_1.html
    20250716_145123_variation_2.html
    20250716_145123_variation_3.html
```

## Technical Considerations
- Uses semantic HTML5 elements
- Implements CSS Grid and Flexbox for layouts
- Includes CSS custom properties for theming
- Follows WCAG accessibility guidelines
- Responsive breakpoints for mobile, tablet, desktop
- Cross-browser compatibility considerations
- Performance optimization techniques