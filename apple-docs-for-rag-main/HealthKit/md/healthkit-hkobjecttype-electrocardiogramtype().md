

- HealthKit
- HKObjectType
-  electrocardiogramType() 

Type Method

# electrocardiogramType()

Returns the shared electrocardiogram type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class func electrocardiogramType() -> HKElectrocardiogramType
```

## Return Value

The shared HKElectrocardiogramType instance.

## Discussion

This method returns an instance of the HKElectrocardiogramType concrete subclass. Use this type to request permission to read HKElectrocardiogram objects from the HealthKit store.

Note

You can’t request permission to share HKActivitySummary objects.

