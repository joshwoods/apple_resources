

- User Notifications
- UNNotificationSound
-  init(named:) 

Initializer

# init(named:)

Creates a sound object that represents a custom sound file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
convenience init(named name: UNNotificationSoundName)
```

## Parameters 

`name`  

The name of the sound file to play. This parameter must not be `nil`.

## Return Value

A sound object representing the custom sound.

## Discussion

This method searches for sound files in the following locations, in order:

1.  The *\*`/Library/Sounds` directory, where *\* is the app’s container directory.

2.  The *\*`/Library/Sounds` directory, where *\* is one of the app’s shared group container directories. For information about how to configure group containers for your app, see Configure app groups.

3.  The main bundle of the current executable.

The method chooses the first file it finds with the specified name.

## See Also

### Creating Notification Sounds

class var `default`: UNNotificationSound

Returns an object representing the default sound for notifications.

