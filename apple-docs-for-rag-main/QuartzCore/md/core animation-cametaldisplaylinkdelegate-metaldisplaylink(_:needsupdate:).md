

- Core Animation
- CAMetalDisplayLinkDelegate
-  metalDisplayLink(\_:needsUpdate:) 

Instance Method

# metalDisplayLink(\_:needsUpdate:)

A method the system calls to notify your app when it plans to update the display.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func metalDisplayLink(
    _ link: CAMetalDisplayLink,
    needsUpdate update: CAMetalDisplayLink.Update
)
```

**Required**

## Parameters 

`link`  

A Metal display link instance the system notifies.

`update`  

An update instance that contains the time the system intends to update the display, a CAMetalDrawable instance, and a deadline to call its present() method.

## Discussion

In this method’s implementation, perform your app’s rendering on the layer or texture of the `update` instance’s drawable property. Before calling present(), encode all your Metal commands to the `link` parameter’s MTLDevice. The GPU has additional time to complete running your commands before the frame displays on screen, determined by the value of the `link` parameter’s preferredFrameLatency property.

Warning

Using alternative methods to present() that target the presentation for a specific time cause an assert when used with a CAMetalDisplayLink.

