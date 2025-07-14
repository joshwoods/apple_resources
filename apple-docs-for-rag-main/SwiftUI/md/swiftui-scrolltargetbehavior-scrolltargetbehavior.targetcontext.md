

- SwiftUI
- ScrollTargetBehavior
-  ScrollTargetBehavior.TargetContext 

Type Alias

# ScrollTargetBehavior.TargetContext

The context in which a scroll behavior updates the scroll target.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias TargetContext = ScrollTargetBehaviorContext
```

## See Also

### Updating the proposed target

func updateTarget(inout ScrollTarget, context: Self.TargetContext)

Updates the proposed target that a scrollable view should scroll to.

**Required**

