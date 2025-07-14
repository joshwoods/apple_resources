

- Core Text
- CTFontManagerScope
-  CTFontManagerScope.process 

Case

# CTFontManagerScope.process

The font is available to the current process for the duration of the process unless directly unregistered.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case process
```

## See Also

### Constants

case none

No scope is defined.

case persistent

The font is available to all processes for the current user session and will be available in subsequent sessions unless unregistered.

case session

The font is available to the current user session but won’t be available in subsequent sessions.

static var user: CTFontManagerScope

The font is available to all processes for the current user session and will be available in subsequent sessions unless unregistered.

