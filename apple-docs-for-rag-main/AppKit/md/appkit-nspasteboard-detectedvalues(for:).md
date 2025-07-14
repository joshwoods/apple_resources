

- AppKit
- NSPasteboard
-  detectedValues(for:) 

Instance Method

# detectedValues(for:)

Determines whether the first pasteboard item matches the specified patterns, reading the contents if it finds a match.

macOS 15.4+

``` source
func detectedValues(for keyPaths: Set>) async throws -> NSPasteboard.DetectedValues
```

## Parameters 

`keyPaths`  

The patterns whose values to detect on the pasteboard.

## Return Value

An object containing the values for the patterns that were detected on the pasteboard.

## Discussion

Important

Calling this method notifies the user that the app has read the contents of the pasteboard, if a match is found.

For details about the types returned for each pattern, see `NSPasteboard.DetectedValues`.

