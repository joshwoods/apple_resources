

- Core Data
- NSEntityDescription
-  subentitiesByName 

Instance Property

# subentitiesByName

A dictionary containing the receiver’s sub-entities.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var subentitiesByName: [String : NSEntityDescription] { get }
```

## Return Value

The keys in the dictionary are the sub-entity names, the corresponding values are instances of `NSEntityDescription`.

## See Also

### Managing inheritance

var subentities: [NSEntityDescription]

An array containing the sub-entities of the receiver.

var superentity: NSEntityDescription?

The super-entity of the receiver.

func isKindOf(entity: NSEntityDescription) -> Bool

Returns a Boolean value that indicates whether the receiver is a sub-entity of another given entity.

