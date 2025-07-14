

- ActivityKit
-  AlertConfiguration 

Structure

# AlertConfiguration

A structure you use to configure an alert that appears when you update your Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
struct AlertConfiguration
```

## Mentioned in 

Displaying live data with Live Activities

## Topics

### Configuring Live Activity alerts

init(title: LocalizedStringResource, body: LocalizedStringResource, sound: AlertConfiguration.AlertSound)

Initializes a new alert configuration for a Live Activity update.

var title: LocalizedStringResource

A short title that describes the purpose of the Live Activity update on Apple Watch.

var body: LocalizedStringResource

The main text that appears on the alert for a Live Activity update on Apple Watch.

var sound: AlertConfiguration.AlertSound

The sound the system plays when the Live Activity alert appears on a person’s device.

struct AlertSound

An object that describes the sound to play for a Live Activity update alert.

### Operators

static func == (AlertConfiguration, AlertConfiguration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Updating a Live Activity

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>) async

Updates the dynamic content of the Live Activity.

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

func update(using: Activity&lt;Attributes>.ContentState) async

Updates the dynamic content of the Live Activity.

Deprecated

func update(ActivityContent&lt;Activity&lt;Attributes>.ContentState>, alertConfiguration: AlertConfiguration?, timestamp: Date) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

