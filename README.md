# Complexity Community Themes

A collection of community-contributed themes for the [Complexity browser extension](https://github.com/pnd280/complexity).

## About

This repository serves as a centralized hub for sharing custom themes created by the Complexity community. Users can discover, preview, and install themes created by other community members.

## Theme Structure

Each theme is stored as a JSON file that follows the `Theme` interface defined in the Complexity extension. A theme consists of:

- `id`: Unique identifier (alphanumeric and hyphens only)
- `title`: Display name of the theme
- `description`: Optional description of the theme
- `displayBannerColors`: Array of colors for theme preview
- `css`: Final CSS styles for the theme
- `config`: Optional configuration object with customization options

## Contributing a Theme

### Method 1: Manual Submission

1. Fork this repository
2. Create a new JSON file in the `themes/` directory
3. Name your file using the pattern: `theme-name.json`
4. Follow the theme schema (see example below)
5. Submit a pull request

### Method 2: Using the Extension (Coming Soon)

The Complexity extension will include a built-in theme submission form that automates the contribution process.

## Theme Example

```json
{
  "id": "midnight-purple",
  "title": "Midnight Purple",
  "description": "A dark theme with purple accents for nighttime browsing",
  "displayBannerColors": ["#1a1625", "#6b46c1", "#8b5cf6"],
  "css": ":root { --accent-color: #8b5cf6; --bg-color: #1a1625; }",
  "config": {
    "title": "Midnight Purple",
    "accentColorSelection": "custom",
    "accentColor": "#8b5cf6",
    "enhanceThreadTypography": true
  }
}
```

## Guidelines

- Theme IDs must be unique and contain only letters, numbers, and hyphens
- Keep theme files under 50KB
- Test your theme thoroughly before submitting
- Provide a meaningful description
- Use appropriate display banner colors that represent your theme

## License

All themes contributed to this repository are licensed under the MIT License, the same as the Complexity extension.

## Support

If you encounter issues with themes or have questions about contributing:
- Open an issue in this repository
- Join the [Complexity community discussions](https://github.com/pnd280/complexity/discussions)
