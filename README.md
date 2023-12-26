# Home Assistant Shelly Multiclick

This integration is a fork of the [built-in Shelly integration](https://github.com/home-assistant/core/tree/dev/homeassistant/components/shelly) of Home Assistant. It overrides some functionality to allow detecting multi-click events.

The code is originally based on this [PR](https://github.com/home-assistant/core/pull/58436), which unfortunately got declined.

This integration includes the patches from then, adapted to the changes that happened to the integration since then.

## Create a New Diff

To re-apply changes to the latest upstream version, create a git diff between the original code and the changes made. This helps to retrace the changes for future updates

```console
git diff upstream-commit-sha changed-commit-sha custom_components/shelly > diff-history/changes-version.diff
```

e.g.,

```console
git diff ca8a055b1678e74ea16adc10cd72b08debb1bf17 091a3372f678e222edb5dc3e913c162b75d57900 > diff-history/changes-2023-4-5.diff
```

To compare between a specific tag and current HEAD, run the following

```console
git diff upstream-2023.12.3 custom_components/shelly > diff-history/changes-2023-12-3.diff
```
