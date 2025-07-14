

- AppKit
- NSUserInterfaceCompressionOptions
-  init(identifier:) 

Initializer

# init(identifier:)

Creates an option object with the given identifier string.

macOS 10.13+

``` source
init(identifier: String)
```

## Discussion

Use this initializer to create custom compression options.

## See Also

### Creating a compression option

init()

Creates an option object containing no options.

init(options: Set&lt;NSUserInterfaceCompressionOptions>)

Creates an option object that represents the union of the supplied options.

init(coder: NSCoder)

Creates an option object from data in an unarchiver.

