

- Media Player
- MPMediaLibrary
-  endGeneratingLibraryChangeNotifications() 

Instance Method

# endGeneratingLibraryChangeNotifications()

Asks the media library to turn off notifications for whenever the library changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func endGeneratingLibraryChangeNotifications()
```

## Discussion

To completely turn off notifications, you must call this method the same number of times that you called beginGeneratingLibraryChangeNotifications().

## See Also

### Receiving notifications when the user’s library changes

func beginGeneratingLibraryChangeNotifications()

Asks the media library to turn on notifications for whenever the library changes.

var lastModifiedDate: Date

The calendar date on which the media library was last modified.

