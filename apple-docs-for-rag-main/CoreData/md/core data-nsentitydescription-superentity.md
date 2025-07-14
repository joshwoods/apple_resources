

- Core Data
- NSEntityDescription
-  superentity 

Instance Property

# superentity

The super-entity of the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var superentity: NSEntityDescription? { get }
```

## Discussion

If the receiver has no super-entity, returns `nil`.

## See Also

### Managing inheritance

var subentitiesByName: [String : NSEntityDescription]

A dictionary containing the receiver’s sub-entities.

var subentities: [NSEntityDescription]

An array containing the sub-entities of the receiver.

func isKindOf(entity: NSEntityDescription) -> Bool

Returns a Boolean value that indicates whether the receiver is a sub-entity of another given entity.

