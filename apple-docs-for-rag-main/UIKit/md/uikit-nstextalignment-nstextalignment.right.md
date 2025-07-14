

- UIKit
- NSTextAlignment
-  NSTextAlignment.right 

Case

# NSTextAlignment.right

Text is right-aligned.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case right
```

## Discussion

The value of this enumeration case is `2` for binaries built for the `arm64` architecture, and running in iOS, macOS, or Simulator. The value is also `2` for binaries built for the `x86_64` architecture and running in Simulator for iOS. However, the value of this enumeration case is `1` for other binaries built for the `x86_64` architecture, including apps translated using Rosetta. If you persist this value manually, make sure to convert it for the appropriate environment when you read it.

For more information about Rosetta, see About the Rosetta translation environment.

## See Also

### Constants

case left

Text is left-aligned.

case center

Text is center-aligned.

case justified

Text is justified.

case natural

Text uses the default alignment for the current localization of the app.

