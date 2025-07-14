

- Network
- NWEndpoint
- NWEndpoint.Port
-  init(\_:) 

Initializer

# init(\_:)

Initializes a port with a string.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init?(_ service: String)
```

## Discussion

Port strings are expected to be numeric values between 0 and 65535. Initializing with any other string will fail.

