

- Game Controller
- GCPhysicalInputProfile
-  mappedPhysicalInputNames(forElementAlias:) 

Instance Method

# mappedPhysicalInputNames(forElementAlias:)

Returns the physical input elements to which the user remaps the given input element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func mappedPhysicalInputNames(forElementAlias elementAlias: String) -> Set
```

## Parameters 

`elementAlias`  

The name of the input element too which physical input elements remap. For possible values, see Extended gamepad input names.

## Return Value

The names of the physical input element to which the user remaps the given element.

## Discussion

For example, if the user maps a physical press of A button , B button, and X button to button B, then passing GCInputButtonB returns a set that contains GCInputButtonA, GCInputButtonB, and GCInputButtonX.

## See Also

### Remapping input elements

var hasRemappedElements: Bool

A Boolean value that indicates whether the user remaps elements in this profile.

func mappedElementAlias(forPhysicalInputName: String) -> String

Returns the name of the input element to which the user remaps the given physical element.

static let GCControllerUserCustomizationsDidChange: NSNotification.Name

A notification that posts when the user customizes the button mappings or other settings of a controller.

