

- CarPlay
-  CPImageSet 

Class

# CPImageSet

Light and dark representations of an image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPImageSet
```

## Overview

CarPlay is set to dark appearance by default in most vehicles, but does provide the option to automatically switch between dark and light appearance. Use an image set to provide images for both appearances, and CarPlay displays the correct one for the current appearance.

## Topics

### Creating an Image Set

init(lightContentImage: UIImage, darkContentImage: UIImage)

Creates an image set with light and dark versions of an image.

### Getting Content Images

var lightContentImage: UIImage

The image the system displays when the user interface style is light.

var darkContentImage: UIImage

The image the system displays when the user interface style is dark.

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
- NSObjectProtocol
- NSSecureCoding

## See Also

### Related Types

class CPButton

A button that displays an image and invokes a handler when the user taps it.

let CarPlayErrorDomain: String

The domain that CarPlay uses for any errors it provides.

