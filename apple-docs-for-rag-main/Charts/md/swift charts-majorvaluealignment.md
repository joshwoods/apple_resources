

- Swift Charts
-  MajorValueAlignment 

Structure

# MajorValueAlignment

A type that defines how the valigned aligned chart scroll target behavior aligns to major values on swipe.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct MajorValueAlignment where Value : Plottable
```

## Topics

### Type Properties

static var page: MajorValueAlignment&lt;Value>

Automatically set the major aligment unit to be the size of the visible domain which is equivalent to a page.

### Type Methods

static func matching(DateComponents) -> MajorValueAlignment&lt;Value>

Align to calendar components.

static func unit(Value) -> MajorValueAlignment&lt;Value>

Align to units.

## See Also

### Supporting types

struct ValueAlignedLimitBehavior

A type that defines the amount of marks that can be scrolled at a time.

struct ValueAlignedChartScrollTargetBehavior

A scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

