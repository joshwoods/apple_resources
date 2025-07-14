

- UIKit
- UIBarAppearance
-  init() 

Initializer

# init()

Creates a new bar appearance object containing default values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init()
```

## Return Value

A new bar appearance object containing default values for the current device idiom.

## See Also

### Creating a custom bar appearance object

init(idiom: UIUserInterfaceIdiom)

Creates a new bar appearance object that targets the specified idiom.

init(barAppearance: UIBarAppearance)

Creates a new bar appearance object by copying relevant data from the specified appearance object.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

