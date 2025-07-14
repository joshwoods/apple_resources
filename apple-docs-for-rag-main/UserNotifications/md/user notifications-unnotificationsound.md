

- User Notifications
-  UNNotificationSound 

Class

# UNNotificationSound

The sound played upon delivery of a notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationSound
```

## Mentioned in 

Generating a remote notification

## Overview

Create a UNNotificationSound object when you want the system to play a specific sound when it delivers with your notification. To play the default system sound, create your sound object using the default method. If you want to play a custom sound, create a new sound object and specify the name of the audio file that you want to play.

For local notifications, assign the sound object to the sound property of your UNMutableNotificationContent object. For a remote notification, assign the name of your sound file to the `sound` key in the `aps` dictionary. You can also use a notification service app extension to add a sound file to a notification shortly before delivery. In your extension, create a UNNotificationSound object and add it to your notification content in the same way that you’d for a local notification.

Audio files must already be on the user’s device before the system can play them. If you use a predefined set of sounds for your notifications, include the audio files in your app’s bundle. For all other sounds, the UNNotificationSound object looks only in the following locations:

- The `/Library/Sounds` directory of the app’s container directory.

- The `/Library/Sounds` directory of one of the app’s shared group container directories.

- The main bundle of the current executable.

### Prepare Sound Resources

The system sound facility plays custom alert sounds, so they must be in one of the following audio data formats:

- Linear PCM

- MA4 (IMA/ADPCM)

- µLaw

- aLaw

You can package the audio data in an `aiff`, `wav`, or `caf` file. Sound files must be less than 30 seconds in length. If the sound file is longer than 30 seconds, the system plays the default sound instead.

You can use the `afconvert` command-line tool to convert sounds. For example, to convert the system sound `Submarine.aiff` to IMA4 audio in a CAF file, use the following command in Terminal:

`afconvert /System/Library/Sounds/Submarine.aiff ~/Desktop/sub.caf -d ima4 -f caff -v`

## Topics

### Creating Notification Sounds

class var `default`: UNNotificationSound

Returns an object representing the default sound for notifications.

convenience init(named: UNNotificationSoundName)

Creates a sound object that represents a custom sound file.

### Getting Critical Sounds

class var defaultCritical: UNNotificationSound

The default sound used for critical alerts.

class func defaultCriticalSound(withAudioVolume: Float) -> Self

Creates a sound object that plays the default critical alert sound at the volume you specify.

class func criticalSoundNamed(UNNotificationSoundName) -> Self

Creates a custom sound object for critical alerts.

class func criticalSoundNamed(UNNotificationSoundName, withAudioVolume: Float) -> Self

Creates a custom sound object for critical alerts with the volume you specify.

### Type Properties

class var defaultRingtone: UNNotificationSound

### Type Methods

class func ringtoneSoundNamed(UNNotificationSoundName) -> Self

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Notification content

Implementing communication notifications

Configure and display your app’s communication notifications by using intents.

protocol UNNotificationContentProviding

A protocol the system uses to provide context relevant to user notifications.

class UNNotificationActionIcon

An icon associated with an action.

class UNMutableNotificationContent

The editable content for a notification.

class UNNotificationContent

The uneditable content of a notification.

class UNNotificationAttachment

A media file associated with a notification.

struct UNNotificationSoundName

A string providing the name of a sound file.

