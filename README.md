# [tools.json](https://cecekpawon.github.io/revanced-tools-api/tools.json)
Auto update `Revanced` Tools API like official https://releases.revanced.app/tools

```
curl -s https://cecekpawon.github.io/revanced-tools-api/tools.json | \
  jq -r  '.[] | map(select(.label == "patches_jar"))[] | .version'
```
