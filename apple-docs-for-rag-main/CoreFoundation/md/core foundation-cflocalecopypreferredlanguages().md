

- Core Foundation
-  CFLocaleCopyPreferredLanguages() 

Function

# CFLocaleCopyPreferredLanguages()

Returns the array of canonicalized language IDs that the user prefers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFLocaleCopyPreferredLanguages() -> CFArray!
```

## Return Value

The array of canonicalized `CFString` language IDs that the current user prefers. Ownership follows the The Create Rule.

