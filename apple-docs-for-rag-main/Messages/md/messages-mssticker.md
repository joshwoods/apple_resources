

- Messages
-  MSSticker 

Class

# MSSticker

A sticker that can be sent as a new message or attached to an existing balloon in the Messages app’s transcript.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
class MSSticker
```

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Topics

### Creating Stickers

init(contentsOfFileURL: URL, localizedDescription: String) throws

Initializes a sticker with the contents of the URL and the localized description.

### Reading Sticker Data

var imageFileURL: URL

The file URL of the image displayed by the sticker.

var localizedDescription: String

The sticker’s localized description.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Message content

class MSConversation

An object that represents a conversation in the Messages app.

