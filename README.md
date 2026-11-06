# Fusion badges

Grey media badges with regex filters for Fusion. 20 badges in one style: resolution, IMAX, HDR, audio formats, channels, subtitles, rating and audio description.

![Preview](preview.png)

## Import

Import this file's raw link in Fusion:

```
https://raw.githubusercontent.com/MohammadSall/gookoo-badges/main/fusion-badges.json
```

## Files

- `fusion-badges.json` holds the filters. Each one has a case-insensitive `pattern` matched against the release name and an `imageURL` pointing into `badges/`.
- `badges/` holds the PNG images: transparent, grey (#C6C6C8), 160 px tall.

## Matching

The patterns follow [Vidhin05/Releases-Regex](https://github.com/Vidhin05/Releases-Regex). Audio, Dolby Vision, resolution and channel badges use the same tag rules as the AIOStreams parser that repo builds on. Each audio badge also skips the formats Vidhin ranks above it, so a file shows one codec badge. IMAX and AD use Vidhin's own patterns.
