

- AppKit
- NSFontManager
-  convertAttributes(\_:) 

Instance Method

# convertAttributes(\_:)

Converts attributes in response to an object initiating an attribute change, typically the Font panel or Font menu.

macOS

``` source
func convertAttributes(_ attributes: [String : Any] = [:]) -> [String : Any]
```

## Parameters 

`attributes`  

The current attributes.

## Return Value

The converted attributes, or `attributes` itself if the conversion isn’t possible.

## Discussion

Attributes unused by the sender should not be changed or removed.

This method is usually invoked on the sender of changeAttributes(_:). See Working with the Font Manager for more information.

## See Also

### Setting Attributes

func setSelectedAttributes([String : Any], isMultiple: Bool)

Informs the Font panel that the specified font attributes changed for the selected text.

