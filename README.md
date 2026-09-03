# Accessibility

MUI components are designed to be accessible to as many people as possible out of the box.

## Overview

Accessibility (a11y) is an essential aspect of web development. MUI includes built-in accessibility features adhering to WAI-ARIA standards.

## Key Features

- **Keyboard Navigation**: All interactive components support standard keyboard interactions (Tab, Enter, Space, Arrow keys).
- **Focus Management**: Focus states are explicitly styled using `:focus-visible` to ensure visibility for keyboard users while preserving standard mouse interactions.
- **Screen Reader Support**: Proper ARIA roles and labels are included across visual elements.

## Best Practices

1. **Icon Buttons**: Always provide an `aria-label` or `aria-labelledby` for buttons containing only icons.
   ```jsx
   <IconButton aria-label="delete">
     <DeleteIcon />
   </IconButton>
   ```
2. **Color Contrast**: Ensure custom color palettes meet WCAG 2.1 AA standards (minimum 4.5:1 contrast ratio for normal text).
3. **Form Controls**: Always associate `<InputLabel>` or provide `aria-label` for standalone inputs.
4. **Target Sizes**: Ensure interactive elements maintain a minimum touch target size of 44x44px for touch interfaces.