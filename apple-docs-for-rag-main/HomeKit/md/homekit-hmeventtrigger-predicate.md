

- HomeKit
- HMEventTrigger
-  predicate 

Instance Property

# predicate

The predicate to evaluate before executing the scene associated with the event trigger.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var predicate: NSPredicate? { get }
```

## Discussion

By default, the value of this property is `nil`, which means that it evaluates as true.

## See Also

### Adding a trigger condition

func updatePredicate(NSPredicate?, completionHandler: ((any Error)?) -> Void)

Replaces the predicate used to evaluate execution of the scene associated with the event trigger.

