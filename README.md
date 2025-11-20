# Corellium Action

This uploads and executes code on a Corellium instance.

# Usage

```yaml
steps:
- uses: plawnekjx/corellium-action@v4
- with:
    token: ${{ secrets.GITHUB_TOKEN }}
    gateway: corellium.plawnekjx.re
    device: android-arm64
    upload: runner.tar.gz
    run: |
      cd /data/android/plawnekjx
      tar xf $ASSET_PATH
      ./gum-tests
```
