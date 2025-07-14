

- UIKit
- UIBarAppearance
-  init(idiom:) 

Initializer

# init(idiom:)

Creates a new bar appearance object that targets the specified idiom.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(idiom: UIUserInterfaceIdiom)
```

## Parameters 

`idiom`  

The device idiom to target. If you specify an idiom that doesn’t make sense for the current device, this method adjusts the idiom to an appropriate value.

## Return Value

A new bar appearance object containing default values for the specified idiom.

## See Also

### Creating a custom bar appearance object

init(barAppearance: UIBarAppearance)

Creates a new bar appearance object by copying relevant data from the specified appearance object.

convenience init()

Creates a new bar appearance object containing default values.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

