

- Foundation
- NSClassDescription
-  register(\_:for:) 

Type Method

# register(\_:for:)

Registers an `NSClassDescription` object for a given class in the `NSClassDescription` cache.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func register(
    _ description: NSClassDescription,
    for aClass: AnyClass
)
```

## Parameters 

`description`  

The class description to register.

`aClass`  

The class for which to register `description`.

## Discussion

You should rarely need to directly invoke this method.

## See Also

### Working with class descriptions

init?(for: AnyClass)

Returns the class description for a given class.

class func invalidateClassDescriptionCache()

Removes all `NSClassDescription` objects from the cache.

