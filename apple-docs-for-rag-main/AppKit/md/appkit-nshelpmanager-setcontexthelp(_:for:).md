

- AppKit
- NSHelpManager
-  setContextHelp(\_:for:) 

Instance Method

# setContextHelp(\_:for:)

Associates help content with an object.

macOS

``` source
@MainActor
func setContextHelp(
    _ attrString: NSAttributedString,
    for object: Any
)
```

## Parameters 

`attrString`  

Help content to associate with `object`.

`object`  

Object to associate with `help`.

## Discussion

When the application enters context-sensitive help mode, if `object` is clicked, `help` appears in the context-sensitive help window.

## See Also

### Configuring Context-Sensitive Help

func removeContextHelp(for: Any)

Removes the association between an object and its context-sensitive help.

