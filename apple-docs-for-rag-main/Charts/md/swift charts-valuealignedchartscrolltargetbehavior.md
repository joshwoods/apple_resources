

- Swift Charts
-  ValueAlignedChartScrollTargetBehavior 

Structure

# ValueAlignedChartScrollTargetBehavior

A scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ValueAlignedChartScrollTargetBehavior
```

## Topics

### Initializers

init(matching: DateComponents, majorAlignment: MajorValueAlignment&lt;Date>?, limitBehavior: ValueAlignedLimitBehavior)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

init&lt;T>(unit: T, majorAlignment: MajorValueAlignment&lt;T>?, limitBehavior: ValueAlignedLimitBehavior)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

init(xMatching: DateComponents, yMatching: DateComponents, xMajorAlignment: MajorValueAlignment&lt;Date>?, yMajorAlignment: MajorValueAlignment&lt;Date>?, limitBehavior: ValueAlignedLimitBehavior)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

init&lt;Y>(xMatching: DateComponents, yUnit: Y, xMajorAlignment: MajorValueAlignment&lt;Date>?, yMajorAlignment: MajorValueAlignment&lt;Y>?, limitBehavior: ValueAlignedLimitBehavior)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

init&lt;X>(xUnit: X, yMatching: DateComponents, xMajorAlignment: MajorValueAlignment&lt;X>?, yMajorAlignment: MajorValueAlignment&lt;Date>?, limitBehavior: ValueAlignedLimitBehavior)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

init&lt;X, Y>(xUnit: X, yUnit: Y, xMajorAlignment: MajorValueAlignment&lt;X>?, yMajorAlignment: MajorValueAlignment&lt;Y>?, limitBehavior: ValueAlignedLimitBehavior)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

## Relationships

### Conforms To

- ChartScrollTargetBehavior
- ScrollTargetBehavior

## See Also

### Supporting types

struct MajorValueAlignment

A type that defines how the valigned aligned chart scroll target behavior aligns to major values on swipe.

struct ValueAlignedLimitBehavior

A type that defines the amount of marks that can be scrolled at a time.

