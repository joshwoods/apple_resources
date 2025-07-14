

- MusicKit
- Album
-  artistName 

Instance Property

# artistName

The artist’s name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var artistName: String { get }
```

## Discussion

You can find more precise information about this album’s artists in the artists relationship, which, unlike artistName, requires that you load it explicitly using the with(_:) method, as in the following example:

```
```

