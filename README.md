# Guiziweb Sylius Recipes

Symfony Flex recipes for Guiziweb Sylius bundles.

## Usage

Add this endpoint to your project's `composer.json`:

```json
{
    "extra": {
        "symfony": {
            "endpoint": [
                "https://api.github.com/repos/Guiziweb/SyliusRecipes/contents/index.json?ref=main",
                "https://api.github.com/repos/Sylius/SyliusRecipes/contents/index.json?ref=flex/main",
                "flex://defaults"
            ]
        }
    }
}
```

Then install any Guiziweb bundle:

```bash
composer require guiziweb/sylius-ai-platform-bundle
```

The recipe will automatically configure:
- Bundle registration in `config/bundles.php`
- Package configuration in `config/packages/`
- Routes in `config/routes/`

## Available Recipes

- `guiziweb/sylius-ai-platform-bundle` - AI Platform infrastructure bundle for Sylius

## Contributing

To add a new recipe, create a PR with the recipe structure in the appropriate directory.