

- SwiftUI
- NSHostingSceneBridgingOptions
-  title 

Type Property

# title

The hosting view’s associated window will have its title and subtitle populated with the values provided to the `navigationTitle(_:)` and `navigationSubtitle(_:)` modifiers, respectively.

macOS 14.0+

``` source
static let title: NSHostingSceneBridgingOptions
```

## Discussion

Title bars populated in this manner overwrite any values set using AppKit.

## See Also

### Geting bridging options

static let all: NSHostingSceneBridgingOptions

The hosting view’s associated window will have both its title bars and toolbars populated with values from their respective modifiers.

static let toolbars: NSHostingSceneBridgingOptions

The hosting view’s associated window will have its toolbar populated with any items provided to the `toolbar(content:)` modifier.

