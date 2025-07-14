

- Core Data
- NSEntityDescription
-  isKindOf(entity:) 

Instance Method

# isKindOf(entity:)

Returns a Boolean value that indicates whether the receiver is a sub-entity of another given entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func isKindOf(entity: NSEntityDescription) -> Bool
```

## Parameters 

`entity`  

An entity.

## Return Value

true if the receiver is a sub-entity of `entity`, otherwise false.

## See Also

### Managing inheritance

var subentitiesByName: [String : NSEntityDescription]

A dictionary containing the receiver’s sub-entities.

var subentities: [NSEntityDescription]

An array containing the sub-entities of the receiver.

var superentity: NSEntityDescription?

The super-entity of the receiver.

