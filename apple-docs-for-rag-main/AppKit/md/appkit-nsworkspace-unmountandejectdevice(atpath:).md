

- AppKit
- NSWorkspace
-  unmountAndEjectDevice(atPath:) 

Instance Method

# unmountAndEjectDevice(atPath:)

Unmounts and ejects the device at the specified path.

macOS

``` source
func unmountAndEjectDevice(atPath path: String) -> Bool
```

## Parameters 

`path`  

The path to the device.

## Return Value

true if the system unmounted the device; otherwise, false.

## Discussion

When this method begins, it posts an willUnmountNotification to the `NSWorkspace` object’s notification center. When it is finished, it posts an didUnmountNotification.

Prefer the unmountAndEjectDevice(at:) method because it provides more detailed error information.

You can safely call this method from any thread of your app.

## See Also

### Unmounting a Device

func unmountAndEjectDevice(at: URL) throws

Attempts to eject the volume mounted at the given path.

