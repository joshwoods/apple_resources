

- SwiftUI
- NSHostingSceneBridgingOptions
-  all 

Type Property

# all

The hosting view’s associated window will have both its title bars and toolbars populated with values from their respective modifiers.

macOS 14.0+

``` source
static let all: NSHostingSceneBridgingOptions
```

## See Also

### Geting bridging options

static let title: NSHostingSceneBridgingOptions

The hosting view’s associated window will have its title and subtitle populated with the values provided to the `navigationTitle(_:)` and `navigationSubtitle(_:)` modifiers, respectively.

static let toolbars: NSHostingSceneBridgingOptions

The hosting view’s associated window will have its toolbar populated with any items provided to the `toolbar(content:)` modifier.

