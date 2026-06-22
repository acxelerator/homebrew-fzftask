# homebrew-fzftask

Homebrew tap for [fzftask](https://github.com/acxelerator/fzftask) — an
fzf-style terminal UI for browsing and running [Taskfile](https://taskfile.dev/)
tasks.

## Install

```bash
brew tap acxelerator/fzftask
brew trust acxelerator/fzftask   # Homebrew 6.0+ requires trusting third-party taps
brew install fzftask
```

Or in one line:

```bash
brew install acxelerator/fzftask/fzftask
```

To build the latest `main` instead of the released version:

```bash
brew install --HEAD acxelerator/fzftask/fzftask
```

## Updating the formula

The formula builds from source and pins the release source tarball's checksum.
For a new version, bump `url` and `sha256` in
[`Formula/fzftask.rb`](Formula/fzftask.rb). The app repo's release workflow
prints the source `sha256` in its release notes, or compute it manually:

```bash
curl -sL https://github.com/acxelerator/fzftask/archive/refs/tags/vX.Y.Z.tar.gz | shasum -a 256
```
