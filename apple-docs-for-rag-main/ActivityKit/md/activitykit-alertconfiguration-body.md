

- ActivityKit
- AlertConfiguration
-  body 

Instance Property

# body

The main text that appears on the alert for a Live Activity update on Apple Watch.

iOS 16.1+iPadOS 16.1+

``` source
var body: LocalizedStringResource
```

## Discussion

Apple Watch displays this string briefly as part of the alert that appears when you update a Live Activity and choose to alert people about the update. Choose text that’s easy to read at a glance. For example, a pizza delivery app could use “Your order will arrive in 25 minutes.”

## See Also

### Configuring Live Activity alerts

init(title: LocalizedStringResource, body: LocalizedStringResource, sound: AlertConfiguration.AlertSound)

Initializes a new alert configuration for a Live Activity update.

var title: LocalizedStringResource

A short title that describes the purpose of the Live Activity update on Apple Watch.

var sound: AlertConfiguration.AlertSound

The sound the system plays when the Live Activity alert appears on a person’s device.

struct AlertSound

An object that describes the sound to play for a Live Activity update alert.

