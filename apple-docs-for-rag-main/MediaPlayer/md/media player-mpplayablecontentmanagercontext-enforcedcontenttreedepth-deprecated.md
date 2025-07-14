

- Media Player
- MPPlayableContentManagerContext
-  enforcedContentTreeDepth Deprecated

Instance Property

# enforcedContentTreeDepth

The maximum depth of the navigation hierarchy allowed by the content server.

iOS 8.4–14.0DeprecatediPadOS 8.4–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var enforcedContentTreeDepth: Int { get }
```

Deprecated

Use CarPlay framework

## Discussion

Exceeding the limit contained by this property causes your app to terminate.

## See Also

### Inspecting content manager properties

var contentLimitsEnforced: Bool

A Boolean value that indicates whether the content server enforces content limits.

Deprecated

var endpointAvailable: Bool

Returns a Boolean that indicates whether the content server is available.

Deprecated

var enforcedContentItemsCount: Int

Returns the number of content items to display during content limiting.

Deprecated

var contentLimitsEnabled: Bool

A Boolean value that indicates whether the content server enables content limits.

Deprecated

