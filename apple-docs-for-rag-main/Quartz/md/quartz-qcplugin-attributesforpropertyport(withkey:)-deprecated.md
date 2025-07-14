

- Quartz
- QCPlugIn
-  attributesForPropertyPort(withKey:) Deprecated

Type Method

# attributesForPropertyPort(withKey:)

Returns a dictionary that contains strings for the user interface that describe the optional attributes for ports created from properties.

macOS 10.4–10.15Deprecated

``` source
class func attributesForPropertyPort(withKey key: String!) -> [AnyHashable : Any]!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The name of the property.

## Return Value

A dictionary that contains key-value pairs for the port’s attributes. The keys must be one or more of the constants defined in Input and Output Port Attributes.

## Discussion

It’s recommended that you implement this method to enhance the experience of those who use your custom patch. The attributes appear in a help tag when the user hovers a pointer over the property port on your custom patch. At a minimum, you should provide a user-readable name for the port. It might also be helpful to provide default, minimum, and maximum values for the port.

## See Also

### Defining Patch and Property Port Attributes

class func attributes() -> [AnyHashable : Any]!

Returns a dictionary that contains strings for the user interface that describe the custom patch.

Deprecated

