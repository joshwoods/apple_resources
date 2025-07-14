

- ActivityKit
- AlertConfiguration
-  sound 

Instance Property

# sound

The sound the system plays when the Live Activity alert appears on a person’s device.

iOS 16.1+iPadOS 16.1+

``` source
var sound: AlertConfiguration.AlertSound
```

## See Also

### Configuring Live Activity alerts

init(title: LocalizedStringResource, body: LocalizedStringResource, sound: AlertConfiguration.AlertSound)

Initializes a new alert configuration for a Live Activity update.

var title: LocalizedStringResource

A short title that describes the purpose of the Live Activity update on Apple Watch.

var body: LocalizedStringResource

The main text that appears on the alert for a Live Activity update on Apple Watch.

struct AlertSound

An object that describes the sound to play for a Live Activity update alert.

