

- Core Data
- NSManagedObjectContext
-  propagatesDeletesAtEndOfEvent 

Instance Property

# propagatesDeletesAtEndOfEvent

A Boolean value that indicates whether the context propagates deletes at the end of the event in which a change was made.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var propagatesDeletesAtEndOfEvent: Bool { get set }
```

## Discussion

true if the receiver propagates deletes at the end of the event in which a change was made, false if it propagates deletes only during a save operation. The default is true.

