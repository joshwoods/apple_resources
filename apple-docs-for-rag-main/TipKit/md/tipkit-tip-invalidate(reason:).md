

- TipKit
- Tip
-  invalidate(reason:) 

Instance Method

# invalidate(reason:)

Permanently invalidates a tip and prevents it from displaying.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func invalidate(reason: Self.InvalidationReason)
```

## Parameters 

`reason`  

The reason for the tip’s invalidation. The tip’s `invalidationReason` returns this value after invalidation.

