

- AppKit
- NSHelpManager
-  removeContextHelp(for:) 

Instance Method

# removeContextHelp(for:)

Removes the association between an object and its context-sensitive help.

macOS

``` source
@MainActor
func removeContextHelp(for object: Any)
```

## Parameters 

`object`  

Object to disassociate from its help content.

## Discussion

If `object` does not have context-sensitive help associated with it, this method does nothing.

## See Also

### Configuring Context-Sensitive Help

func setContextHelp(NSAttributedString, for: Any)

Associates help content with an object.

