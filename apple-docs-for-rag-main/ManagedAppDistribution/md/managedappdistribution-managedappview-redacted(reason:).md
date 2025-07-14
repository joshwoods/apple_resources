

- ManagedAppDistribution
- ManagedAppView
-  redacted(reason:) 

Instance Method

# redacted(reason:)

Adds a reason to apply a redaction to this view hierarchy.

ManagedAppDistributionSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func redacted(reason: RedactionReasons) -> some View
```

## Discussion

Adding a redaction is an additive process: any redaction provided will be added to the reasons provided by the parent.

