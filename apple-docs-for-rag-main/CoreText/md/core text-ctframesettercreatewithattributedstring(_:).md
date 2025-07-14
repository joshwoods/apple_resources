

- Core Text
-  CTFramesetterCreateWithAttributedString(\_:) 

Function

# CTFramesetterCreateWithAttributedString(\_:)

Creates an immutable framesetter object from an attributed string.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFramesetterCreateWithAttributedString(_ attrString: CFAttributedString) -> CTFramesetter
```

## Parameters 

`attrString`  

The attributed string for constructing the framesetter object.

## Return Value

A reference to a framesetter object if the call is successful; otherwise, `NULL`.

## Discussion

Use the framesetter object to create and fill text frames with the CTFramesetterCreateFrame(_:_:_:_:) call.

Note

By default, the text system doesn’t typeset text that requires an unreasonable amount of effort. To create a framesetter that supports typesetting text regardless of the amount of effort necessary, create a CTTypesetter with the kCTTypesetterOptionAllowUnboundedLayout option set to kCFBooleanTrue, then use CTFramesetterCreateWithTypesetter(_:) instead.

## See Also

### Creating a Framesetter

func CTFramesetterCreateWithTypesetter(CTTypesetter) -> CTFramesetter

Creates a framesetter directly from a typesetter.

