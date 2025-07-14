

- Core Animation
- CAMetalLayer
-  displaySyncEnabled 

Instance Property

# displaySyncEnabled

A Boolean value that determines whether the layer synchronizes its updates to the display’s refresh rate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.13+

``` source
var displaySyncEnabled: Bool { get set }
```

## Discussion

Set this value to true to synchronize the presentation of the layer’s contents with the display’s refresh, also known as *vsync* or *vertical sync*. If false, the layer presents new content more quickly, but possibly with brief visual artifacts (*screen tearing*).

The default value is true.

## See Also

### Configuring Presentation Behavior

var presentsWithTransaction: Bool

A Boolean value that determines whether the layer presents its content using a Core Animation transaction.

