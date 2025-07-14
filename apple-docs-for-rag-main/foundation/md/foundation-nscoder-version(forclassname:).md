

- Foundation
- NSCoder
-  version(forClassName:) 

Instance Method

# version(forClassName:)

This method is present for historical reasons and is not used with keyed archivers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func version(forClassName className: String) -> Int
```

## Return Value

The version in effect for the class named `className` or `NSNotFound` if no class named `className` exists.

## Discussion

The version number does apply not to `NSKeyedArchiver`/`NSKeyedUnarchiver`. A keyed archiver does not encode class version numbers.

## See Also

### Getting Version Information

var systemVersion: UInt32

The system version in effect for the archive.

