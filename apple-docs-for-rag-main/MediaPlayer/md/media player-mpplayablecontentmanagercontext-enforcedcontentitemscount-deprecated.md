

- Media Player
- MPPlayableContentManagerContext
-  enforcedContentItemsCount Deprecated

Instance Property

# enforcedContentItemsCount

Returns the number of content items to display during content limiting.

iOS 8.4–14.0DeprecatediPadOS 8.4–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var enforcedContentItemsCount: Int { get }
```

Deprecated

Use CarPlay framework

## Discussion

This property returns NSIntegerMax when the content server doesn’t limit the maximum number of items.

## See Also

### Inspecting content manager properties

var contentLimitsEnforced: Bool

A Boolean value that indicates whether the content server enforces content limits.

Deprecated

var endpointAvailable: Bool

Returns a Boolean that indicates whether the content server is available.

Deprecated

var enforcedContentTreeDepth: Int

The maximum depth of the navigation hierarchy allowed by the content server.

Deprecated

var contentLimitsEnabled: Bool

A Boolean value that indicates whether the content server enables content limits.

Deprecated

