

- AppKit
- NSFontManager
-  setSelectedAttributes(\_:isMultiple:) 

Instance Method

# setSelectedAttributes(\_:isMultiple:)

Informs the Font panel that the specified font attributes changed for the selected text.

macOS

``` source
func setSelectedAttributes(
    _ attributes: [String : Any],
    isMultiple flag: Bool
)
```

## Parameters 

`attributes`  

The new attributes.

`flag`  

If true, informs the panel that multiple fonts or attributes are enclosed within the selection.

## Discussion

This method is used primarily by `NSTextView`.

## See Also

### Setting Attributes

func convertAttributes([String : Any]) -> [String : Any]

Converts attributes in response to an object initiating an attribute change, typically the Font panel or Font menu.

