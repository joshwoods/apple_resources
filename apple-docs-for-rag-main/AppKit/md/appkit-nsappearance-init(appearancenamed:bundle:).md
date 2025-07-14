

- AppKit
- NSAppearance
-  init(appearanceNamed:bundle:) 

Initializer

# init(appearanceNamed:bundle:)

Creates an appearance object from the named appearance file located in the specified bundle.

macOS 10.9+

``` source
init?(
    appearanceNamed name: NSAppearance.Name,
    bundle: Bundle?
)
```

## Parameters 

`name`  

The name of the appearance file to retrieve. Do not include any path information in the name.

`bundle`  

The bundle in which to search for the named appearance file. Specify `nil` to search for the appearance file in the main bundle.

## Return Value

An initialized appearance object, or `nil` if an error occurs.

## See Also

### Creating an Appearance

init?(named: NSAppearance.Name)

Creates an appearance object based on the name of one of the standard system appearances.

init?(coder: NSCoder)

