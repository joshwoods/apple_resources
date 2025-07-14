

- UIKit
- UIBarAppearance
-  init(coder:) 

Initializer

# init(coder:)

Creates an appearance object from data in an unarchiver.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(coder: NSCoder)
```

## See Also

### Creating a custom bar appearance object

init(idiom: UIUserInterfaceIdiom)

Creates a new bar appearance object that targets the specified idiom.

init(barAppearance: UIBarAppearance)

Creates a new bar appearance object by copying relevant data from the specified appearance object.

convenience init()

Creates a new bar appearance object containing default values.

