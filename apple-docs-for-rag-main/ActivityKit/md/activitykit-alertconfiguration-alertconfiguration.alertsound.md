

- ActivityKit
- AlertConfiguration
-  AlertConfiguration.AlertSound 

Structure

# AlertConfiguration.AlertSound

An object that describes the sound to play for a Live Activity update alert.

iOS 16.1+iPadOS 16.1+

``` source
struct AlertSound
```

## Topics

### Configuring the alert sound

static func named(String) -> AlertConfiguration.AlertSound

A function you use to configure a custom sound for a Live Activity update alert.

static var `default`: AlertConfiguration.AlertSound

A value that represents the system’s default alert sound.

### Operators

static func == (AlertConfiguration.AlertSound, AlertConfiguration.AlertSound) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Configuring Live Activity alerts

init(title: LocalizedStringResource, body: LocalizedStringResource, sound: AlertConfiguration.AlertSound)

Initializes a new alert configuration for a Live Activity update.

var title: LocalizedStringResource

A short title that describes the purpose of the Live Activity update on Apple Watch.

var body: LocalizedStringResource

The main text that appears on the alert for a Live Activity update on Apple Watch.

var sound: AlertConfiguration.AlertSound

The sound the system plays when the Live Activity alert appears on a person’s device.

