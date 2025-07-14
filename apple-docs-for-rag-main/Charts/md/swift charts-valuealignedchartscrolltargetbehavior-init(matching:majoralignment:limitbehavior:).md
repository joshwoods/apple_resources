

- Swift Charts
- ValueAlignedChartScrollTargetBehavior
-  init(matching:majorAlignment:limitBehavior:) 

Initializer

# init(matching:majorAlignment:limitBehavior:)

Creates a scroll target behavior that aligns to values spaced at regular intervals along the scrollable axes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    matching components: DateComponents,
    majorAlignment: MajorValueAlignment? = nil,
    limitBehavior: ValueAlignedLimitBehavior = .automatic
)
```

## Parameters 

`components`  

The components to search for when aligning after the user finishes scrolling.

`majorAlignment`  

The behavior for aligning to major values. When the user swipes on the chart, the chart will snap to the next or previous major unit depending on the swipe direction. When enabled, the default major unit is a page.

`limitBehavior`  

The scroll limit behavior.

