

- UIKit
- UIInputViewController
-  primaryLanguage 

Instance Property

# primaryLanguage

The primary language for a custom keyboard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var primaryLanguage: String? { get set }
```

## Discussion

A BCP 47 language identifier, such as `en-US`. If specified, this value supersedes the `PrimaryLanguage` key in a custom keyboard’s `Info.plist` file.

