

- AppKit
- NSSplitViewController
-  viewDidLoad() 

Instance Method

# viewDidLoad()

Configures the split view controller after its view loads into memory.

macOS 10.10+

``` source
@MainActor
func viewDidLoad()
```

## Discussion

NSSplitViewController overrides this method from its parent class, NSViewController. If you override this method in a subclass, you must call `super`.

