

- AVFoundation
- AVMediaSelectionGroup
-  options 

Instance Property

# options

A collection of mutually exclusive media selection options

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var options: [AVMediaSelectionOption] { get }
```

## Discussion

The value of the property is an array of AVMediaSelectionOption objects.

## See Also

### Accessing Media Selection Options

func mediaSelectionOption(withPropertyList: Any) -> AVMediaSelectionOption?

Returns the media selection options that match the given property list.

var defaultOption: AVMediaSelectionOption?

The default option in the group.

