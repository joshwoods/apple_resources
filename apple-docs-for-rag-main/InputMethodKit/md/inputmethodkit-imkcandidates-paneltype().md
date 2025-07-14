

- InputMethodKit
- IMKCandidates
-  panelType() 

Instance Method

# panelType()

Returns the style of the candidates window.

macOS 10.5+

``` source
@MainActor
func panelType() -> IMKCandidatePanelType
```

## Return Value

A IMKCandidatePanelType constant that represents the style of the candidates window.

## See Also

### Managing Window Type and Text Attributes

func setPanelType(IMKCandidatePanelType)

Sets the style of the candidates window.

func setAttributes([AnyHashable : Any]!)

Sets the style attributes for the candidates window.

func attributes() -> [AnyHashable : Any]!

Returns a dictionary of the style attributes used for the candidates window..

