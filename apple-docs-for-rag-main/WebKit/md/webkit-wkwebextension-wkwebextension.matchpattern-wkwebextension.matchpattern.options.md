

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  WKWebExtension.MatchPattern.Options 

Structure

# WKWebExtension.MatchPattern.Options

Constants used by WKWebExtension.MatchPattern to indicate matching options.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct Options
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var ignorePaths: WKWebExtension.MatchPattern.Options

Indicates that the host components should be ignored while matching.

static var ignoreSchemes: WKWebExtension.MatchPattern.Options

Indicates that the scheme components should be ignored while matching.

static var matchBidirectionally: WKWebExtension.MatchPattern.Options

Indicates that two patterns should be checked in either direction while matching.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

