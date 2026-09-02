# Last9RUM (Swift Package Manager)

Real User Monitoring for iOS apps, distributed as a binary `Last9RUM.xcframework`.

This repository is a thin, auto-generated Swift Package Manager wrapper around
the xcframework published to the Last9 CDN. It exists so you can add the SDK in
Xcode by URL instead of managing a `.binaryTarget` checksum by hand.

Full setup, configuration and changelog live in the
[Last9 iOS RUM docs](https://last9.io/docs/discover-applications/).

## Install

In Xcode: **File → Add Package Dependencies…**, paste this repository's URL,
then choose a dependency rule:

- **Exact Version (recommended for a frozen build):** pin exactly `1.6.9-alpha.33595414494`.
- **Branch `stable/vN`:** always resolve the latest non-breaking release
  within major version `N`.

```swift
// Package.swift consumers — pin an exact version…
.package(url: "https://github.com/last9/last9-rum-ios.git", exact: "1.6.9-alpha.33595414494")
// …or track the stable branch for the latest non-breaking release:
// .package(url: "https://github.com/last9/last9-rum-ios.git", branch: "stable/v1")
```

Then `import Last9RUM`. See the docs for token setup and initialization.

<!-- generated: channel=version version=1.6.9-alpha.33595414494 -->
