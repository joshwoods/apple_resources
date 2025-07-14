

- Foundation
- NSClassDescription
-  invalidateClassDescriptionCache() 

Type Method

# invalidateClassDescriptionCache()

Removes all `NSClassDescription` objects from the cache.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func invalidateClassDescriptionCache()
```

## Discussion

You should rarely need to invoke this method. Use it whenever a registered `NSClassDescription` object might be replaced by a different version, such as when you have loaded a new provider of `NSClassDescription` objects, or when you are about to remove a provider of `NSClassDescription` objects.

## See Also

### Working with class descriptions

init?(for: AnyClass)

Returns the class description for a given class.

class func register(NSClassDescription, for: AnyClass)

Registers an `NSClassDescription` object for a given class in the `NSClassDescription` cache.

