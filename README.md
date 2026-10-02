# ItsReidar Homebrew Tap

Homebrew casks for apps by [ItsReidar](https://github.com/ItsReidar).

## Brain.md

A Markdown notes editor with live preview and a built-in MCP server. Requires macOS 26 (Tahoe) or later.

```bash
brew install --cask itsreidar/tap/brain-md
```

Brain.md is signed but not notarized by Apple, so macOS blocks its first launch, and the first launch after each upgrade. Allow it in one of these ways:

- Open the app once, then go to **System Settings > Privacy & Security** and click **Open Anyway**.
- Or remove the download quarantine flag in Terminal. `sudo` isn't needed, because Homebrew installs the app under your user:

  ```bash
  xattr -dr com.apple.quarantine /Applications/brain-md.app
  ```

Upgrade with `brew upgrade --cask brain-md`.

## Maintenance

Casks in `Casks/` are generated and published by the release scripts in [ItsReidar/brain-md](https://github.com/ItsReidar/brain-md/blob/main/docs/releasing.md). Don't edit them by hand.
