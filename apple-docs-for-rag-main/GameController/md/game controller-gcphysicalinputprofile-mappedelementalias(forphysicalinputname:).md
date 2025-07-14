

- Game Controller
- GCPhysicalInputProfile
-  mappedElementAlias(forPhysicalInputName:) 

Instance Method

# mappedElementAlias(forPhysicalInputName:)

Returns the name of the input element to which the user remaps the given physical element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func mappedElementAlias(forPhysicalInputName inputName: String) -> String
```

## Parameters 

`inputName`  

The name of the physical element. For possible values, see Extended gamepad input names.

## Return Value

The name of the input element to which the user remaps the physical element, or `nil` if the user doesn’t remap the physical element.

## Discussion

Use this method to get the alias for an input element. For example, if the user remaps a physical press of the controller’s A button to button B, then passing GCInputButtonA to this method returns GCInputButtonB.

## See Also

### Remapping input elements

var hasRemappedElements: Bool

A Boolean value that indicates whether the user remaps elements in this profile.

func mappedPhysicalInputNames(forElementAlias: String) -> Set&lt;String>

Returns the physical input elements to which the user remaps the given input element.

static let GCControllerUserCustomizationsDidChange: NSNotification.Name

A notification that posts when the user customizes the button mappings or other settings of a controller.

