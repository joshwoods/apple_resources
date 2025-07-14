

- AVFoundation
- AVCaptureMetadataInput
-  init(formatDescription:clock:) 

Initializer

# init(formatDescription:clock:)

Creates capture metadata input to provide timed groups to a capture session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
init(
    formatDescription desc: CMMetadataFormatDescription,
    clock: CMClock
)
```

## Parameters 

`desc`  

A CMFormatDescription that defines the metadata to be supplied by the client. Throws invalidArgumentException if `NULL` is passed.

`clock`  

A doc://com.apple.documentation/documentation/coremedia/cmclock-u5q that provides the timebase for the supplied samples. Throws invalidArgumentException if `NULL` is passed.

