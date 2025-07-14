

- Media Player
-  MPMusicPlayerPlayParameters 

Class

# MPMusicPlayerPlayParameters

The MusicKit parameters that describe items to play.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerPlayParameters
```

## Topics

### Creating the play parameters

init?(dictionary: [String : Any])

Returns a new play parameters object using information from MusicKit.

### Accessing the play parameters

var dictionary: [String : Any]

The information returned from a MusicKit query and stored in a play parameters object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating a new play parameters queue descriptor

init(playParametersQueue: [MPMusicPlayerPlayParameters])

Creates a new queue descriptor using the designated queue of play parameters.

