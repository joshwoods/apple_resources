

- AVFoundation
- AVDateRangeMetadataGroup
-  init(items:start:end:) 

Initializer

# init(items:start:end:)

Initializes an instance of `AVDateRangeMetadataGroup` with a collection of metadata items.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    items: [AVMetadataItem],
    start startDate: Date,
    end endDate: Date?
)
```

## Parameters 

`items`  

The array of AVMetadataItem instances to associate with this group.

`startDate`  

The starting date for the group of metadata items.

`endDate`  

The ending date for the group of metadata items.

## Return Value

A new instance of `AVDateRangeMetadataGroup`.

## Discussion

Creates a new instance of `AVDateRangeMetadataGroup` with the specified collection of metadata items. The `startDate` and `endDate` arguments define the effective time range on the timeline to which the metadata applies.

