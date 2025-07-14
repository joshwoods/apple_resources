

- InputMethodKit
- IMKCandidates
-  selectionKeys() 

Instance Method

# selectionKeys()

Returns an array of `NSNumber` objects where each `NSNumber` object represents a virtual key code.

macOS 10.5+

``` source
@MainActor
func selectionKeys() -> [Any]!
```

## Return Value

The array of `NSNumber` objects.

## Discussion

Selection keys are keys that can be used to select one of the candidates. They are displayed next to the candidate that will be selected when the user types that key.

## See Also

### Managing Selection Keys

func setSelectionKeys([Any]!)

Sets the selection keys for the candidates.

func setSelectionKeysKeylayout(TISInputSource!)

Sets the key layout that is used to map virtual key codes to characters.

func selectionKeysKeylayout() -> Unmanaged&lt;TISInputSource>!

Returns the key layout that maps virtual key codes to selection keys.

