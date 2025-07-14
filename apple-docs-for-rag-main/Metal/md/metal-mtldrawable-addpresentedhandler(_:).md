

- Metal
- MTLDrawable
-  addPresentedHandler(\_:) 

Instance Method

# addPresentedHandler(\_:)

Registers a block of code to be called immediately after the drawable is presented.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.4+macOS 10.15.4+tvOS 10.2+visionOS 1.0+

``` source
func addPresentedHandler(_ block: @escaping MTLDrawablePresentedHandler)
```

**Required**

## Parameters 

`block`  

A block of code to be invoked.

## Discussion

You can register multiple handlers for a single drawable object.

The following example code schedules a presentation handler that reads the presentedTime property and uses it to derive the interval between the last and current presentation times. From that information, it determines the app’s frame rate.

- Swift
- Objective-C

```
// Property declarations
var previousPresentedTime: CFTimeInterval = 0.0
/* ... */
// Render loop
currentDrawable.addPresentedHandler({ [weak self] drawable in
    guard let strongSelf = self else {
        return
    }
    let presentationDuration = drawable.presentedTime - strongSelf.previousPresentedTime
    let frameRate = 1.0/presentationDuration
    /* ... */
    strongSelf.previousPresentedTime = drawable.presentedTime
})
```

```
// Property declarations
@property (nonatomic) CFTimeInterval previousPresentedTime;
/* ... */
// Render loop
__block Renderer *strongSelf = self;
[view.currentDrawable addPresentedHandler:^(id drawable) {
    CFTimeInterval presentationDuration = drawable.presentedTime - strongSelf.previousPresentedTime;
    CFTimeInterval frameRate = 1.0/presentationDuration;
    /* ... */
    strongSelf.previousPresentedTime = drawable.presentedTime;
}];
```

## See Also

### Getting Presentation Information

var presentedTime: CFTimeInterval

The host time, in seconds, when the drawable was displayed onscreen.

**Required**

