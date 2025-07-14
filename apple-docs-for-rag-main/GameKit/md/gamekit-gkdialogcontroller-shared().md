

- GameKit
- GKDialogController
-  shared() 

Type Method

# shared()

Retrieves the shared instance of the dialog controller.

macOS 10.8+

``` source
@MainActor
class func shared() -> GKDialogController
```

## Return Value

The shared dialog controller.

## Discussion

You can use the shared dialog controller or create your own GKDialogController object. For example, you can create separate GKDialogController objects for different windows.

