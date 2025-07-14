

- System
- CInterop
-  CInterop.PlatformChar 

Type Alias

# CInterop.PlatformChar

The platform’s preferred character type. On Unix, this is an 8-bit C `char` (which may be signed or unsigned, depending on platform). On Windows, this is `UInt16` (a “wide” character).

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias PlatformChar = CInterop.Char
```

