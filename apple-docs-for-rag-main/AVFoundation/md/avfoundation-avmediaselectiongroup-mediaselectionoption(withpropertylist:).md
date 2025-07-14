

- AVFoundation
- AVMediaSelectionGroup
-  mediaSelectionOption(withPropertyList:) 

Instance Method

# mediaSelectionOption(withPropertyList:)

Returns the media selection options that match the given property list.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func mediaSelectionOption(withPropertyList plist: Any) -> AVMediaSelectionOption?
```

## Parameters 

`plist`  

A property list previously obtained from an option in the group using propertyList() (`AVMediaSelectionOption`).

## Return Value

An AVMediaSelectionOption object containing the properites passed by `plist`. Returns `nil` when no match is found.

## See Also

### Accessing Media Selection Options

var options: [AVMediaSelectionOption]

A collection of mutually exclusive media selection options

var defaultOption: AVMediaSelectionOption?

The default option in the group.

