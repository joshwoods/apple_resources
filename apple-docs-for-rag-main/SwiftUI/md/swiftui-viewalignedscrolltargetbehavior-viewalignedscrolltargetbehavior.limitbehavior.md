

- SwiftUI
- ViewAlignedScrollTargetBehavior
-  ViewAlignedScrollTargetBehavior.LimitBehavior 

Structure

# ViewAlignedScrollTargetBehavior.LimitBehavior

A type that defines the amount of views that can be scrolled at a time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct LimitBehavior
```

## Topics

### Getting the limit behavior

static var automatic: ViewAlignedScrollTargetBehavior.LimitBehavior

The automatic limit behavior.

static var always: ViewAlignedScrollTargetBehavior.LimitBehavior

The always limit behavior.

static var never: ViewAlignedScrollTargetBehavior.LimitBehavior

The never limit behavior.

### Type Properties

static var alwaysByFew: ViewAlignedScrollTargetBehavior.LimitBehavior

The always-by-few limit behavior.

static var alwaysByOne: ViewAlignedScrollTargetBehavior.LimitBehavior

The always-by-one limit behavior.

## See Also

### Creating the target behavior

init(limitBehavior: ViewAlignedScrollTargetBehavior.LimitBehavior)

Creates a view aligned scroll behavior.

