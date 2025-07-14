

- AppKit
- NSAppearance
-  init(named:) 

Initializer

# init(named:)

Creates an appearance object based on the name of one of the standard system appearances.

macOS 10.9+

``` source
init?(named name: NSAppearance.Name)
```

## Parameters 

`name`  

The name of a standard appearance. See NSAppearance.Name for the list of standard appearance names.

## Return Value

A standard NSAppearance object.

## Discussion

When you specify a standard appearance name—such as aqua—this method returns a built-in appearance.

## See Also

### Creating an Appearance

init?(appearanceNamed: NSAppearance.Name, bundle: Bundle?)

Creates an appearance object from the named appearance file located in the specified bundle.

init?(coder: NSCoder)

