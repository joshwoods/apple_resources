

- Core Image
- CIFilterGenerator
-  removeExportedKey(\_:) 

Instance Method

# removeExportedKey(\_:)

Removes a key that was previously exported.

macOS 10.5+

``` source
func removeExportedKey(_ exportedKeyName: String)
```

## Parameters 

`exportedKeyName`  

The name of the key you want to remove.

## See Also

### Managing Exported Keys

var exportedKeys: [AnyHashable : Any]

Returns an array of the exported keys.

func exportKey(String, from: Any, withName: String?)

Exports an input or output key of an object in the filter chain.

func setAttributes([AnyHashable : Any], forExportedKey: String)

Sets a dictionary of attributes for an exported key.

