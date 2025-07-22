# Discussion #37059

## Current behavior

```json

    {
      "description": "Disable all managers",
      "matchManagers": ["*"],
      "enabled": false
    }

```

does not disable all managers.

## Expected behavior

The configuration should disable all package managers when the `matchManagers` is set to `["*"]` and `enabled` is set to `false`.

I should be able to enable managers selectively after this configuration.

So in this example the `Dockerfile` manager should be enabled, but all others should be disabled. This works for `pre-commit`, but the `tflint` manager is still enabled.

## Link to the Renovate issue or Discussion

[Disussion #37059](https://github.com/renovatebot/renovate/discussions/37059)
