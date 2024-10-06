---
title: Patch YMCA Website Services
---

Here you can find instructions how you can patch YMCA Website Services distribution used on
your project.

## When you need to patch YMCA Website Services

- In case you found a bug and prepared a patch for YMCA Website Services on github.
- In case you developed a new feature that will be good to have in YMCA Website Services and
created Pull Request to YMCA Website Services repository
- In case you want to add a feature that added to YMCA Website Services but not included yet to
YMCA Website Services release.

### How to patch YMCA Website Services via composer?

If you followed instructions [docs/Development/Start new YMCA Website Services project](https://github.com/YCloudYUSA/yusaopeny/blob/8.x-1.x/docs/Development/Start%20new%20OpenY%20project.md)
and you have configured `composer.json` you need just to do a few simple steps:
1. Build a link to a patch using pull request ID

    ```
    https://patch-diff.githubusercontent.com/raw/YCloudYUSA/yusaopeny/pull/XXX.patch
    ```

Where XXX is a number of pull request you want to use.

2. Add a new section `patches` to the section `extra` and add a patch to YMCA Website Services
repository, as on this example:

    ```
    "extra": {
        "installer-paths": {
          ...
        },
        "enable-patching": true,
        "patches": {
            "YCloudYUSA/yusaopeny": {
                "Patch description": "https://patch-diff.githubusercontent.com/raw/YCloudYUSA/yusaopeny/pull/XXX.patch"
            }
        }
    }
    ```

3. After adding a patch execute command `composer update`
4. Verify you can see added changes in YMCA Website Services
5. Enjoy!
