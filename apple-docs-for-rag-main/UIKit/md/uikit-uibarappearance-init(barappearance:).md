

- UIKit
- UIBarAppearance
-  init(barAppearance:) 

Initializer

# init(barAppearance:)

Creates a new bar appearance object by copying relevant data from the specified appearance object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(barAppearance: UIBarAppearance)
```

## Parameters 

`barAppearance`  

The bar appearance object from which to copy the relevant properties.

## Return Value

A new bar appearance object containing the relevant properties from the other object.

## Discussion

This method copies over the properties from `barAppearance` that are also relevant to the new bar appearance object.

## See Also

### Creating a custom bar appearance object

init(idiom: UIUserInterfaceIdiom)

Creates a new bar appearance object that targets the specified idiom.

convenience init()

Creates a new bar appearance object containing default values.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

