

- InputMethodKit
- IMKCandidates
-  setSelectionKeysKeylayout(\_:) 

Instance Method

# setSelectionKeysKeylayout(\_:)

Sets the key layout that is used to map virtual key codes to characters.

macOS 10.5+

``` source
@MainActor
func setSelectionKeysKeylayout(_ layout: TISInputSource!)
```

## Parameters 

`layout`  

The key layout to use.

## See Also

### Managing Selection Keys

func setSelectionKeys([Any]!)

Sets the selection keys for the candidates.

func selectionKeys() -> [Any]!

Returns an array of `NSNumber` objects where each `NSNumber` object represents a virtual key code.

func selectionKeysKeylayout() -> Unmanaged&lt;TISInputSource>!

Returns the key layout that maps virtual key codes to selection keys.

