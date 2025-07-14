

- Core Animation
- CAMetalLayer
-  presentsWithTransaction 

Instance Property

# presentsWithTransaction

A Boolean value that determines whether the layer presents its content using a Core Animation transaction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var presentsWithTransaction: Bool { get set }
```

## Discussion

By default, this value is false; CAMetalLayer displays the output of a rendering pass to the display as quickly as possible and asynchronously to any Core Animation transactions. Core Animation doesn’t guarantee that the Metal content arrives in the same frame as other Core Animation content. This behavior could be an issue if, for example, your app draws UIKit content over the top of your CAMetalLayer.

Setting this value to true makes the layer draw its contents synchronously, using whichever Core Animation transaction is current at the time you call the drawable’s present() method. To ensure that a transaction is available when you schedule the drawable to be presented, first commit the command buffer containing your Metal rendering commands. Then, call its waitUntilScheduled() method to synchronously wait until the command queue schedules the command buffer to execute on the GPU. Finally, call the drawable’s present() method.

Warning

If you’re synchronizing presentation with a Core Animation transaction, don’t use the present(_:) method on the command buffer to schedule the drawable for presentation. This convenience method (and any variant of it on MTLCommandBuffer) doesn’t wait for a transaction to be available.

## See Also

### Configuring Presentation Behavior

var displaySyncEnabled: Bool

A Boolean value that determines whether the layer synchronizes its updates to the display’s refresh rate.

