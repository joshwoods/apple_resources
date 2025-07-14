

- ReplayKit
- RPSystemBroadcastPickerView
-  preferredExtension 

Instance Property

# preferredExtension

A bundle identifier of a broadcast extension.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var preferredExtension: String? { get set }
```

## Discussion

Set this property to the bundle identifier of a broadcast extension to show only that broadcast provider in the broadcast picker. Set the property to `nil`, which is the default value, to show all broadcast providers available on the device.

## See Also

### Configuring the Broadcast Picker

var showsMicrophoneButton: Bool

A Boolean value that indicates whether the microphone button is visible in the broadcast picker.

