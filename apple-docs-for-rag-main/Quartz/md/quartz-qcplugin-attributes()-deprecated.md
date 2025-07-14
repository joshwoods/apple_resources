

- Quartz
- QCPlugIn
-  attributes() Deprecated

Type Method

# attributes()

Returns a dictionary that contains strings for the user interface that describe the custom patch.

macOS 10.4–10.15Deprecated

``` source
class func attributes() -> [AnyHashable : Any]!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The dictionary can contain one or more of these keys along with the appropriate string: QCPlugInAttributeNameKey and QCPlugInAttributeDescriptionKey.

## Discussion

It’s recommended that you implement this method to enhance the experience of those who use your custom patch. The attribute name string that you provide is displayed in the Quartz Composer editor window when the custom patch name is selected in the Patch Creator (see figure). The attribute description key is displayed in the Information pane of the inspector for the custom patch.

## See Also

### Defining Patch and Property Port Attributes

class func attributesForPropertyPort(withKey: String!) -> [AnyHashable : Any]!

Returns a dictionary that contains strings for the user interface that describe the optional attributes for ports created from properties.

Deprecated

