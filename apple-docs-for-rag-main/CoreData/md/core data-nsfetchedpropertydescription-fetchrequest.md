

- Core Data
- NSFetchedPropertyDescription
-  fetchRequest 

Instance Property

# fetchRequest

The fetch request of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fetchRequest: NSFetchRequest? { get set }
```

## Discussion

Setting the fetch request raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Related Documentation

Core Data Programming Guide

Predicate Programming Guide

