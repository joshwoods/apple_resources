

- EventKit
- EKEventStore
-  sources 

Instance Property

# sources

An unordered array of objects that represent accounts that contain calendars.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var sources: [EKSource] { get }
```

## Discussion

Although this property is an array, the order of the elements in the array isn’t guaranteed.

## See Also

### Accessing account sources

var delegateSources: [EKSource]

The event sources delegated to the person using your app.

func source(withIdentifier: String) -> EKSource?

Locates an event source with the specified identifier.

