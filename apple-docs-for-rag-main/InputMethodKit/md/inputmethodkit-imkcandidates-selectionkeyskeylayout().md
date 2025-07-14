

- InputMethodKit
- IMKCandidates
-  selectionKeysKeylayout() 

Instance Method

# selectionKeysKeylayout()

Returns the key layout that maps virtual key codes to selection keys.

macOS 10.5+

``` source
@MainActor
func selectionKeysKeylayout() -> Unmanaged!
```

## Return Value

The key layout in use. By default this is the key layout whose source id is `com.apple.keylayout.US`.

## See Also

### Managing Selection Keys

func setSelectionKeys([Any]!)

Sets the selection keys for the candidates.

func selectionKeys() -> [Any]!

Returns an array of `NSNumber` objects where each `NSNumber` object represents a virtual key code.

func setSelectionKeysKeylayout(TISInputSource!)

Sets the key layout that is used to map virtual key codes to characters.

