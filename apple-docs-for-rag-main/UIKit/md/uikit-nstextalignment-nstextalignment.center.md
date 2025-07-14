

- UIKit
- NSTextAlignment
-  NSTextAlignment.center 

Case

# NSTextAlignment.center

Text is center-aligned.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case center
```

## Discussion

The value of this enumeration case is `1` for binaries built for the `arm64` architecture, and running in iOS, macOS, or Simulator. The value is also `1` for binaries built for the `x86_64` architecture and running in Simulator for iOS. However, the value of this enumeration case is `2` for other binaries built for the `x86_64` architecture, including apps translated using Rosetta. If you persist this value manually, make sure to convert it for the appropriate environment when you read it.

For more information about Rosetta, see About the Rosetta translation environment.

## See Also

### Constants

case left

Text is left-aligned.

case right

Text is right-aligned.

case justified

Text is justified.

case natural

Text uses the default alignment for the current localization of the app.

