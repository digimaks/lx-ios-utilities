# UtilitiesPackage

Shared utilities for iOS — typed access to `UserDefaults`, including App Group suites.

It is one of the Swift packages used by **Digimaks**, a mobile digital wallet
continuing the work of the
[NOBID Consortium](https://www.nobidconsortium.com/) (the Nordic-Baltic eID
Project), one of the EU Large Scale Pilots preparing for eIDAS 2.0.

## Background

This package is the continuation of
[nobid-lsp-latvia/lx-ios-utilities](https://github.com/nobid-lsp-latvia/lx-ios-utilities),
developed within the NOBID Consortium and carried forward under the name
**Digimaks**.

## Requirements

- iOS 15+
- Swift 5.9+ / Xcode 15+

## Installation

Add the package to your `Package.swift`:

```swift
.package(url: "<repository-url>", from: "1.0.0")
```

or add it in Xcode via **File → Add Package Dependencies…**.

## Overview

| Type | Responsibility |
| ---- | -------------- |
| `UserDefaultsManager` | Generic `get` / `set` / `remove`, plus `getValueFromSuite` for reading values shared through an App Group |

The suite accessor lets an app and its extensions (for example a share
extension) exchange values through a shared container.

## Licence

Licensed under the [EUPL-1.2](LICENSE). See [Notice](Notice) for attribution.
