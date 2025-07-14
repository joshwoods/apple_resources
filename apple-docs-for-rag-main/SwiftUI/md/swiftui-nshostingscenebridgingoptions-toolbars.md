

- SwiftUI
- NSHostingSceneBridgingOptions
-  toolbars 

Type Property

# toolbars

The hosting view’s associated window will have its toolbar populated with any items provided to the `toolbar(content:)` modifier.

macOS 14.0+

``` source
static let toolbars: NSHostingSceneBridgingOptions
```

## Discussion

Toolbars populated in this manner overwrite any toolbar set on the window using AppKit.

## See Also

### Geting bridging options

static let all: NSHostingSceneBridgingOptions

The hosting view’s associated window will have both its title bars and toolbars populated with values from their respective modifiers.

static let title: NSHostingSceneBridgingOptions

The hosting view’s associated window will have its title and subtitle populated with the values provided to the `navigationTitle(_:)` and `navigationSubtitle(_:)` modifiers, respectively.

