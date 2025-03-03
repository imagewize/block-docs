# Understanding WordPress Style Variations

## What Are Style Variations?

Style variations (like consulting.json, studio.json, and startup.json) allow WordPress themes to provide multiple "looks" or styles using the same underlying theme code. They're an efficient way to create visual variety without duplicating theme files.

## How Style Variations Work

1. **Base Theme + Variations**:
   - `theme.json` provides the foundational styling and defaults
   - Style variations (like consulting.json) only specify what's different from the base theme

2. **Complete Styling System**: 
   - Each style variation is essentially a preset color palette + typography + spacing combination
   - Users can select these without any coding knowledge

## Why Use Both Palettes AND Style Variations?

There are two levels of customization at play:

### Level 1: Style Variations (consulting.json, studio.json)
- Complete "looks" with pre-coordinated design systems
- Each includes its own color palette, button styles, typography choices
- Allows for dramatic changes with one selection
- These are meant to completely transform the site's appearance

### Level 2: Color Palettes (royal-blue.json)
- More granular control over just the colors
- Can be applied regardless of which style variation is active
- Allows changing only colors without affecting typography, spacing, etc.

## Real-World Analogy

Think of it like this:
- Style variations (consulting.json) = Complete outfits (shirt, pants, shoes, accessories)
- Color palettes (royal-blue.json) = Just changing the color of the outfit

## Benefits of This Approach

1. **Efficiency**: Define common elements once in theme.json
2. **Maintainability**: Easier to update the core theme
3. **User Experience**: Offer meaningful design choices without overwhelming users
4. **Performance**: Smaller files since variations only contain differences
5. **Flexibility**: Create new looks by combining variations with color palettes

The reason consulting.json has a full color palette inside it (rather than just referring to royal-blue.json) is that style variations need to be complete, standalone configurations. This ensures the style works perfectly regardless of what other settings the user has applied.
