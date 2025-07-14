

- Core Animation
- CALayer
-  defaultAction(forKey:) 

Type Method

# defaultAction(forKey:)

Returns the default action for the current class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func defaultAction(forKey event: String) -> (any CAAction)?
```

## Parameters 

`event`  

The identifier of the action.

## Return Value

Returns a suitable action object for the given key or `nil` of no action object was associated with that key.

## Discussion

Classes that want to provide default actions can override this method and use it to return those actions.

## See Also

### Getting the Layer’s Actions

func action(forKey: String) -> (any CAAction)?

Returns the action object assigned to the specified key.

var actions: [String : any CAAction]?

A dictionary containing layer actions.

