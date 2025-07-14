

- SwiftUI
- SpringLoadingBehavior
-  automatic 

Type Property

# automatic

The automatic spring loading behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let automatic: SpringLoadingBehavior
```

## Discussion

This defers to default component behavior for spring loading. Some components, such as `TabView`, will default to allowing spring loading; while others do not.

## See Also

### Getting the behaviors

static let enabled: SpringLoadingBehavior

Spring loaded interactions will be enabled for applicable views.

static let disabled: SpringLoadingBehavior

Spring loaded interactions will be disabled for applicable views.

