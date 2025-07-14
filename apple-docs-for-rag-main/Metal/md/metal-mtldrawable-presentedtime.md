

- Metal
- MTLDrawable
-  presentedTime 

Instance Property

# presentedTime

The host time, in seconds, when the drawable was displayed onscreen.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.4+macOS 10.15.4+tvOS 10.2+visionOS 1.0+

``` source
var presentedTime: CFTimeInterval { get }
```

**Required**

## Discussion

Typically, you query this property in a callback method. See addPresentedHandler(_:).

The property value is `0.0` if the drawable hasn’t been presented or if its associated frame was dropped.

## See Also

### Getting Presentation Information

func addPresentedHandler(MTLDrawablePresentedHandler)

Registers a block of code to be called immediately after the drawable is presented.

**Required**

