

- AppKit
- NSStoryboard
-  instantiateInitialController(creator:) 

Instance Method

# instantiateInitialController(creator:)

Creates the initial view controller from the storyboard and initializes it using your custom code.

macOS 10.15+

``` source
func instantiateInitialController(creator: ((NSCoder) -> Controller?)? = nil) -> Controller? where Controller : NSViewController
```

## Parameters 

`creator`  

A block that contains your custom creation code for the view controller. Use this block to create the view controller, initialize it with the provided coder object and any custom information you require, and return the result. This block returns a new view controller object and takes the following parameter:

coder  
The coder object that contains the storyboard data to use when configuring the view controller.

If you return `nil` from your block, this method creates the view controller using the default init(coder:) method.

## Return Value

The initial view controller in the storyboard.

## Discussion

Every storyboard file has an initial controller object that represents the default interface to create. Use this method to construct that object using a custom code that you provide. Use this method when the constructor for your object takes parameters in addition to the specified `coder` object.

In your `creator` block, create the view controller using your custom constructor method. Your custom constructor method must accept an NSCoder parameter and must call the inherited init(coder:) method at some point during its execution. Not doing so is a programmer error.

## See Also

### Loading the Initial View Controller

func instantiateInitialController() -> Any?

Creates the initial view controller or window controller from a storyboard.

func instantiateInitialController&lt;Controller>(creator: ((NSCoder) -> Controller?)?) -> Controller?

Creates the initial window controller from the storyboard and initializes it using your custom code.

