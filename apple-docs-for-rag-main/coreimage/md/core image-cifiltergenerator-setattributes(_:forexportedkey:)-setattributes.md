

- Core Image
- CIFilterGenerator
-  setAttributes(\_:forExportedKey:) 

Instance Method

# setAttributes(\_:forExportedKey:)

Sets a dictionary of attributes for an exported key.

macOS 10.5+

``` source
func setAttributes(
    _ attributes: [AnyHashable : Any],
    forExportedKey key: String
)
```

## Parameters 

`attributes`  

A dictionary that describes the attributes associated with the specified key.

`key`  

The exported key whose attributes you want to set.

## Discussion

By default, the exported key inherits the attributes from its original key and target object. You can use this method to change one or more of the existing attributes for the key, such as the default value or maximum value. For more information on attributes, see CIFilter and Core Image Programming Guide.

## See Also

### Managing Exported Keys

var exportedKeys: [AnyHashable : Any]

Returns an array of the exported keys.

func exportKey(String, from: Any, withName: String?)

Exports an input or output key of an object in the filter chain.

func removeExportedKey(String)

Removes a key that was previously exported.

