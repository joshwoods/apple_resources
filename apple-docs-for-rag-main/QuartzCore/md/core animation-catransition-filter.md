

- Core Animation
- CATransition
-  filter 

Instance Property

# filter

An optional Core Image filter object that provides the transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+

``` source
var filter: Any? { get set }
```

## Discussion

If specified, the filter must support both kCIInputImageKey and kCIInputTargetImageKey input keys, and the kCIOutputImageKey output key. The filter may optionally support the kCIInputExtentKey input key, which is set to a rectangle describing the region in which the transition should run. If `filter` does not support the required input and output keys the behavior is undefined.

Defaults to `nil`. When a transition filter is specified the type and subtype properties are ignored.

The NSView that contains the transitioning layer must have its layerUsesCoreImageFilters set to true.

The following code shows how you can transition between the two states of a CATextLayer named `transitioningLayer`. When the layer is first created, its backgroundColor is set to red and its string property is set to `Red`. When the `runTransition()` function is called, a new CATransition object is created and added to `transitioningLayer`, and the state of the layer is changed so that its background color is blue and its rendered text reads `Blue`.

The end result is that the transition animates from the red state to the blue state using a CICopyMachineTransition transition.

```
override func viewDidLoad() {
    super.viewDidLoad()

    view.layerUsesCoreImageFilters = true

    view.layer = CALayer()

    transitioningLayer.frame = CGRect(x: 10, y: 10,
                                      width: 320, height: 160)

    view.layer!.addSublayer(transitioningLayer)

    // Initial "red" state
    transitioningLayer.backgroundColor = NSColor.red.cgColor
    transitioningLayer.string = "Red"
}

func runTransition() {
    let transition = CATransition()
    transition.duration = 2

    transition.filter = CIFilter(name: "CICopyMachineTransition")
    transitioningLayer.add(transition,
                           forKey: "transition")

    // Transition to "blue" state
    transitioningLayer.backgroundColor = NSColor.blue.cgColor
    transitioningLayer.string = "Blue"
}
```

### Special Considerations

This property is not supported on layers in iOS.

