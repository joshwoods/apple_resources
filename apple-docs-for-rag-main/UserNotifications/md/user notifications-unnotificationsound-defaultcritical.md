

- User Notifications
- UNNotificationSound
-  defaultCritical 

Type Property

# defaultCritical

The default sound used for critical alerts.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 5.0+

``` source
@NSCopying
class var defaultCritical: UNNotificationSound { get }
```

## Discussion

Critical alerts ingore the mute switch and Do Not Disturb. They require a special entitlement issued by Apple.

## See Also

### Getting Critical Sounds

class func defaultCriticalSound(withAudioVolume: Float) -> Self

Creates a sound object that plays the default critical alert sound at the volume you specify.

class func criticalSoundNamed(UNNotificationSoundName) -> Self

Creates a custom sound object for critical alerts.

class func criticalSoundNamed(UNNotificationSoundName, withAudioVolume: Float) -> Self

Creates a custom sound object for critical alerts with the volume you specify.

