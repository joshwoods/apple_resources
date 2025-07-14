

- AppKit
- NSPasteboard
-  detectedPatterns(for:) 

Instance Method

# detectedPatterns(for:)

Determines whether the first pasteboard item matches the specified patterns, without notifying the user.

macOS 15.4+

``` source
func detectedPatterns(for keyPaths: Set>) async throws -> Set>
```

## Parameters 

`keyPaths`  

The patterns to detect on the pasteboard.

## Return Value

A set with the patterns found on the pasteboard.

## Discussion

Because this method only gives an indication of whether a pasteboard item matches a particular pattern and doesn’t allow the app to access the contents, the system doesn’t notify the user about reading the contents of the pasteboard.

