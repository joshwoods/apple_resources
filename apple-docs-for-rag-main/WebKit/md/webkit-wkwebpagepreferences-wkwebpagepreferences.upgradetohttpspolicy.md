

- WebKit
- WKWebpagePreferences
-  WKWebpagePreferences.UpgradeToHTTPSPolicy 

Enumeration

# WKWebpagePreferences.UpgradeToHTTPSPolicy

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
enum UpgradeToHTTPSPolicy
```

## Overview

Preference for loading a webpage with https, and how failures should be handled.

## Topics

### Enumeration Cases

case automaticFallbackToHTTP

case errorOnFailure

case keepAsRequested

case userMediatedFallbackToHTTP

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

