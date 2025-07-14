

- Swift Charts
-  ChartScrollTargetBehavior 

Protocol

# ChartScrollTargetBehavior

A type that configures the scroll behavior of charts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol ChartScrollTargetBehavior : ScrollTargetBehavior
```

## Topics

### Supporting types

struct MajorValueAlignment

A type that defines how the valigned aligned chart scroll target behavior aligns to major values on swipe.

struct ValueAlignedLimitBehavior

A type that defines the amount of marks that can be scrolled at a time.

struct ValueAlignedChartScrollTargetBehavior

A scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

### Instance Methods

func updateTarget(inout ScrollTarget, context: ChartScrollTargetBehaviorContext)

**Required** Default implementation provided.

### Type Methods

static func valueAligned(matching: DateComponents, majorAlignment: MajorValueAlignment&lt;Date>?, limitBehavior: ValueAlignedLimitBehavior) -> ValueAlignedChartScrollTargetBehavior

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

static func valueAligned&lt;P>(unit: P, majorAlignment: MajorValueAlignment&lt;P>?, limitBehavior: ValueAlignedLimitBehavior) -> ValueAlignedChartScrollTargetBehavior

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

static func valueAligned(xMatching: DateComponents, yMatching: DateComponents, xMajorAlignment: MajorValueAlignment&lt;Date>?, yMajorAlignment: MajorValueAlignment&lt;Date>?, limitBehavior: ValueAlignedLimitBehavior) -> ValueAlignedChartScrollTargetBehavior

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

static func valueAligned&lt;Y>(xMatching: DateComponents, yUnit: Y, xMajorAlignment: MajorValueAlignment&lt;Date>?, yMajorAlignment: MajorValueAlignment&lt;Y>?, limitBehavior: ValueAlignedLimitBehavior) -> ValueAlignedChartScrollTargetBehavior

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

static func valueAligned&lt;X>(xUnit: X, yMatching: DateComponents, xMajorAlignment: MajorValueAlignment&lt;X>?, yMajorAlignment: MajorValueAlignment&lt;Date>?, limitBehavior: ValueAlignedLimitBehavior) -> ValueAlignedChartScrollTargetBehavior

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

static func valueAligned&lt;X, Y>(xUnit: X, yUnit: Y, xMajorAlignment: MajorValueAlignment&lt;X>?, yMajorAlignment: MajorValueAlignment&lt;Y>?, limitBehavior: ValueAlignedLimitBehavior) -> ValueAlignedChartScrollTargetBehavior

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

### Default Implementations

ScrollTargetBehavior Implementations

## Relationships

### Inherits From

- ScrollTargetBehavior

### Conforming Types

- ValueAlignedChartScrollTargetBehavior

## See Also

### Scrolling

struct ChartScrollTargetBehaviorContext

Contextual information that you can use to determine how to best adjust how charts scroll.

