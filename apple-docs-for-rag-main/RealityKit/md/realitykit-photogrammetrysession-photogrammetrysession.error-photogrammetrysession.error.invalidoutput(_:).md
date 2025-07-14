

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Error
-  PhotogrammetrySession.Error.invalidOutput(\_:) 

Case

# PhotogrammetrySession.Error.invalidOutput(\_:)

An error that represents an invalid output location.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
case invalidOutput(URL)
```

## Discussion

This error occurs in two cases:

1.  The URL points to a directory that is not empty.

2.  The URL points to a file ending in ‘.usdz’ that already exists.

