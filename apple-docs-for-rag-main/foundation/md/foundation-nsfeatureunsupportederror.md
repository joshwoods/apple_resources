

- Foundation
-  NSFeatureUnsupportedError 

Global Variable

# NSFeatureUnsupportedError

The feature isn’t supported, because the file system lacks the feature, or required libraries are missing, or other similar reasons.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var NSFeatureUnsupportedError: Int { get }
```

## Discussion

For example, some volumes may not support a Trash folder, so these methods will report failure by returning false or `nil` and an NSError with NSFeatureUnsupportedError.

## See Also

### Miscellaneous Errors

var NSKeyValueValidationError: Int

A key-value coding validation error.

