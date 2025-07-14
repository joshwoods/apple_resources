

- HealthKit
- HKObjectType
-  activitySummaryType() 

Type Method

# activitySummaryType()

Returns the shared activity summary type.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.2+

``` source
class func activitySummaryType() -> HKActivitySummaryType
```

## Return Value

The shared HKActivitySummaryType instance.

## Discussion

This method returns an instance of the HKActivitySummaryType concrete subclass. Use this type to request permission to read HKActivitySummary objects from the HealthKit store.

Note

You cannot request permission to share HKActivitySummary objects.

