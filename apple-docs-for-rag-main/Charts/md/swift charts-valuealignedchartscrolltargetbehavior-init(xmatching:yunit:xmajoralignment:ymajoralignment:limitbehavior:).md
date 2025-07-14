

- Swift Charts
- ValueAlignedChartScrollTargetBehavior
-  init(xMatching:yUnit:xMajorAlignment:yMajorAlignment:limitBehavior:) 

Initializer

# init(xMatching:yUnit:xMajorAlignment:yMajorAlignment:limitBehavior:)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    xMatching xComponents: DateComponents,
    yUnit: Y,
    xMajorAlignment: MajorValueAlignment? = nil,
    yMajorAlignment: MajorValueAlignment? = nil,
    limitBehavior: ValueAlignedLimitBehavior = .automatic
) where Y : Plottable, Y : Numeric
```

## Parameters 

`xComponents`  

The alignment components for the x-axis.

`yUnit`  

The alignment unit for the y-axis.

`xMajorAlignment`  

The behavior for aligning to major values along the x-axis.

`yMajorAlignment`  

The behavior for aligning to major values along the y-axis.

`limitBehavior`  

The scroll limit behavior.

