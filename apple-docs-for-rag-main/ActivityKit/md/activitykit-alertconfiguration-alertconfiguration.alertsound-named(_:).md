

- ActivityKit
- AlertConfiguration
- AlertConfiguration.AlertSound
-  named(\_:) 

Type Method

# named(\_:)

A function you use to configure a custom sound for a Live Activity update alert.

iOS 16.1+iPadOS 16.1+

``` source
static func named(_ name: String) -> AlertConfiguration.AlertSound
```

## Parameters 

`name`  

The name of the sound file to use for the alert. Choose a file that’s in your app’s main bundle or the `Library/Sounds` folder of your app’s data container.

## See Also

### Configuring the alert sound

static var `default`: AlertConfiguration.AlertSound

A value that represents the system’s default alert sound.

