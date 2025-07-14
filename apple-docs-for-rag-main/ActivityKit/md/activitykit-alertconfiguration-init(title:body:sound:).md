

- ActivityKit
- AlertConfiguration
-  init(title:body:sound:) 

Initializer

# init(title:body:sound:)

Initializes a new alert configuration for a Live Activity update.

iOS 16.1+iPadOS 16.1+

``` source
init(
    title: LocalizedStringResource,
    body: LocalizedStringResource,
    sound: AlertConfiguration.AlertSound
)
```

## Parameters 

`title`  

The short title that describes the purpose of the Live Activity update.

`body`  

The main text of the alert for a Live Activity update.

`sound`  

The sound that the system plays when the alert appears on a person’s device.

## See Also

### Configuring Live Activity alerts

var title: LocalizedStringResource

A short title that describes the purpose of the Live Activity update on Apple Watch.

var body: LocalizedStringResource

The main text that appears on the alert for a Live Activity update on Apple Watch.

var sound: AlertConfiguration.AlertSound

The sound the system plays when the Live Activity alert appears on a person’s device.

struct AlertSound

An object that describes the sound to play for a Live Activity update alert.

