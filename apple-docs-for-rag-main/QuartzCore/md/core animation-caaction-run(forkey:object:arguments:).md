

- Core Animation
- CAAction
-  run(forKey:object:arguments:) 

Instance Method

# run(forKey:object:arguments:)

Called to trigger the action specified by the identifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func run(
    forKey event: String,
    object anObject: Any,
    arguments dict: [AnyHashable : Any]?
)
```

**Required**

## Parameters 

`event`  

The identifier of the action. The identifier may be a key or key path relative to `anObject`, an arbitrary external action, or one of the action identifiers defined in CALayer.

`anObject`  

The layer on which the action should occur.

`dict`  

A dictionary containing parameters associated with this event. May be `nil`.

## See Also

### Related Documentation

Core Animation Programming Guide

