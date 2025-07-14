

- Core Text
- CTFontManagerScope
-  user 

Type Property

# user

The font is available to all processes for the current user session and will be available in subsequent sessions unless unregistered.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.6+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var user: CTFontManagerScope { get }
```

## See Also

### Constants

case none

No scope is defined.

case process

The font is available to the current process for the duration of the process unless directly unregistered.

case persistent

The font is available to all processes for the current user session and will be available in subsequent sessions unless unregistered.

case session

The font is available to the current user session but won’t be available in subsequent sessions.

