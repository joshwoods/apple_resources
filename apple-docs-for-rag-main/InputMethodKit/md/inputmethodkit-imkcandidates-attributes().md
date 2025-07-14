

- InputMethodKit
- IMKCandidates
-  attributes() 

Instance Method

# attributes()

Returns a dictionary of the style attributes used for the candidates window..

macOS 10.5+

``` source
@MainActor
func attributes() -> [AnyHashable : Any]!
```

## Return Value

The dictionary that contains the keys and values for the styles.

## See Also

### Managing Window Type and Text Attributes

func panelType() -> IMKCandidatePanelType

Returns the style of the candidates window.

func setPanelType(IMKCandidatePanelType)

Sets the style of the candidates window.

func setAttributes([AnyHashable : Any]!)

Sets the style attributes for the candidates window.

