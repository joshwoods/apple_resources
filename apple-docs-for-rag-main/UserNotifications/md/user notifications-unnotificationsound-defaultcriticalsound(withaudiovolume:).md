

- User Notifications
- UNNotificationSound
-  defaultCriticalSound(withAudioVolume:) 

Type Method

# defaultCriticalSound(withAudioVolume:)

Creates a sound object that plays the default critical alert sound at the volume you specify.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 5.0+

``` source
class func defaultCriticalSound(withAudioVolume volume: Float) -> Self
```

## Parameters 

`volume`  

The volume must be a value between 0.0 and 1.0.

## Return Value

A sound object representing the default critical alert sound at the specified volume.

## Discussion

Critical alerts ignore the mute switch and Do Not Disturb. They require a special entitlement issued by Apple.

## See Also

### Getting Critical Sounds

class var defaultCritical: UNNotificationSound

The default sound used for critical alerts.

class func criticalSoundNamed(UNNotificationSoundName) -> Self

Creates a custom sound object for critical alerts.

class func criticalSoundNamed(UNNotificationSoundName, withAudioVolume: Float) -> Self

Creates a custom sound object for critical alerts with the volume you specify.

