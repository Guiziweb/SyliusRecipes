# Guiziweb Sylius Recipes

Symfony Flex recipes for Guiziweb Sylius plugins.

## Usage

Add this endpoint to your project's `composer.json`:

```json
{
    "extra": {
        "symfony": {
            "endpoint": [
                "https://api.github.com/repos/Guiziweb/SyliusRecipes/contents/index.json?ref=flex/main",
                "flex://defaults"
            ]
        }
    }
}
```

Then install any Guiziweb plugin:

```bash
composer require guiziweb/sylius-grid-assistant-plugin
```

The recipe will automatically configure:
- Bundle registration in `config/bundles.php`
- Package configuration in `config/packages/`
- Routes in `config/routes/`
- Environment variables in `.env`

## Available Recipes

- `guiziweb/sylius-grid-assistant-plugin` - AI-powered natural language filtering for Sylius grids

## Contributing

To add a new recipe, add the recipe structure in the appropriate directory and push to `main`. The `flex/main` branch is updated automatically.