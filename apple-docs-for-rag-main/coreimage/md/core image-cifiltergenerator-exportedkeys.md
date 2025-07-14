

- Core Image
- CIFilterGenerator
-  exportedKeys 

Instance Property

# exportedKeys

Returns an array of the exported keys.

macOS 10.5+

``` source
var exportedKeys: [AnyHashable : Any] { get }
```

## Return Value

An array of dictionaries that describe the exported key and target object. See kCIFilterGeneratorExportedKey, kCIFilterGeneratorExportedKeyTargetObject, and kCIFilterGeneratorExportedKey for keys used in the dictionary.

## Discussion

This method returns the keys that you exported using the exportKey(_:from:withName:) method or that were exported before being written to the file from which you read the filter chain.

## See Also

### Managing Exported Keys

func exportKey(String, from: Any, withName: String?)

Exports an input or output key of an object in the filter chain.

func removeExportedKey(String)

Removes a key that was previously exported.

func setAttributes([AnyHashable : Any], forExportedKey: String)

Sets a dictionary of attributes for an exported key.

