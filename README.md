# recipes

A collection of recipes in YAML format, designed for use with [ByGrams](https://github.com/walnutgeek/bygrams).

## Format

Each recipe is a `.yaml` or `.yml` file following the ByGrams [recipe schema](https://github.com/walnutgeek/bygrams/blob/main/docs/recipe-schema.md). Ingredients use grams as the primary unit where possible, making recipes easy to scale.

## Adding a recipe

Create a YAML file in the repo root (or in a subdirectory for automatic tagging):

```yaml
name: Hummus
src:
  - url: https://example.com/hummus
tags:
  - Appetizer
actions:
  - name: Blend
    ingredients:
      - 400g chickpeas, drained
      - 45g tahini
      - 28g olive oil
      - 15g lemon juice
      - 3 cloves garlic, crushed
      - salt to taste
```

## Gram conversions

Add a `conversions.yaml` to the repo root to define unit-to-gram mappings. See the [schema docs](https://github.com/walnutgeek/bygrams/blob/main/docs/recipe-schema.md#conversions-file) for the format.
