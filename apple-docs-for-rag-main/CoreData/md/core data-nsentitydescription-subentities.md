

- Core Data
- NSEntityDescription
-  subentities 

Instance Property

# subentities

An array containing the sub-entities of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var subentities: [NSEntityDescription] { get set }
```

## Discussion

The sub-entities are instances of `NSEntityDescription`.

### Special Considerations

Setting the sub-entities raises an exception if the receiver’s model has been used by an object graph manager.

## See Also

### Managing inheritance

var subentitiesByName: [String : NSEntityDescription]

A dictionary containing the receiver’s sub-entities.

var superentity: NSEntityDescription?

The super-entity of the receiver.

func isKindOf(entity: NSEntityDescription) -> Bool

Returns a Boolean value that indicates whether the receiver is a sub-entity of another given entity.

