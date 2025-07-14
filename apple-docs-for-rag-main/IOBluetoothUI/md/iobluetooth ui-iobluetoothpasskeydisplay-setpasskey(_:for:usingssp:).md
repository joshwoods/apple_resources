

- IOBluetooth UI
- IOBluetoothPasskeyDisplay
-  setPasskey(\_:for:usingSSP:) 

Instance Method

# setPasskey(\_:for:usingSSP:)

macOS 10.2+

``` source
@MainActor
func setPasskey(
    _ inString: String!,
    for device: IOBluetoothDevice!,
    usingSSP isSSP: Bool
)
```

## See Also

### Instance Methods

func advancePasskeyIndicator()

func resetPasskeyIndicator()

func retreatPasskeyIndicator()

