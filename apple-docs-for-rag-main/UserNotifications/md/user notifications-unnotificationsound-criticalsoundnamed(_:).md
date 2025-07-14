

- User Notifications
- UNNotificationSound
-  criticalSoundNamed(\_:) 

Type Method

# criticalSoundNamed(\_:)

Creates a custom sound object for critical alerts.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
class func criticalSoundNamed(_ name: UNNotificationSoundName) -> Self
```

## Parameters 

`name`  

The name of the sound file to play. This file must be located in the current executable’s main bundle or in the `Library/Sounds` directory of the current app container directory. If files exist at both locations, the system uses the file from the `Library/Sounds` directory. This parameter must not be `nil`.

## Return Value

A sound object representing a custom critical alert sound.

## Discussion

Critical alerts ignore the mute switch and Do Not Disturb. They require a special entitlement issued by Apple.

## See Also

### Getting Critical Sounds

class var defaultCritical: UNNotificationSound

The default sound used for critical alerts.

class func defaultCriticalSound(withAudioVolume: Float) -> Self

Creates a sound object that plays the default critical alert sound at the volume you specify.

class func criticalSoundNamed(UNNotificationSoundName, withAudioVolume: Float) -> Self

Creates a custom sound object for critical alerts with the volume you specify.

