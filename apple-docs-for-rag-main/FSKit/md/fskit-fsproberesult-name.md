

- FSKit
- FSProbeResult
-  name 

Instance Property

# name

The resource name, as found during the probe operation.

macOS 15.4+

``` source
var name: String? { get }
```

## Discussion

This value is non-`nil` unless the result is \`\`FSMatchResult/notRecognized\`. For formats that lack a name, this value may be an empty string. This value can also be an empty string if the format supports a name, but the value isn’t set yet.

## See Also

### Working with result properties

var containerID: FSContainerIdentifier?

The container identifier, as found during the probe operation.

var result: FSMatchResult

The match result, representing the recognition and usability of a probed resource.

enum FSMatchResult

A type that represents the recognition and usability of a probed resource.

