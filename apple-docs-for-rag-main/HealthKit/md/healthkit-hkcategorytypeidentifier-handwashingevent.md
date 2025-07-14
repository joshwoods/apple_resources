

- HealthKit
- HKCategoryTypeIdentifier
-  handwashingEvent 

Type Property

# handwashingEvent

A category sample type for handwashing events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
static let handwashingEvent: HKCategoryTypeIdentifier
```

## Discussion

Use this type to read or share handwashing events. When creating a handwashing event sample, set the value to HKCategoryValue.notApplicable, and set the duration by specifying different start and end dates. The Health app uses the sample’s duration to determine if the handwashing event completed.

Apple Watch automatically detects and records handwashing events on Apple Watch Series 4 and later.

## See Also

### Self care

static let toothbrushingEvent: HKCategoryTypeIdentifier

A category sample type for toothbrushing events.

