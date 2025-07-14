

- Game Controller
- GCVirtualController
-  controller 

Instance Property

# controller

The underlying controller object that you use to access input elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var controller: GCController? { get }
```

## Discussion

Use this property to either get the element’s input values directly, or set handlers to get callbacks with the input values that changed. If you don’t connect the virtual controller to the device using `connect()`, this property is `nil`.

