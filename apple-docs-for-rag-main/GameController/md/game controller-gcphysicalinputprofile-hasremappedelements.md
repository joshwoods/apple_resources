

- Game Controller
- GCPhysicalInputProfile
-  hasRemappedElements 

Instance Property

# hasRemappedElements

A Boolean value that indicates whether the user remaps elements in this profile.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var hasRemappedElements: Bool { get }
```

## Discussion

If true, the user remaps one or more elements; otherwise, this property is false.

## See Also

### Remapping input elements

func mappedElementAlias(forPhysicalInputName: String) -> String

Returns the name of the input element to which the user remaps the given physical element.

func mappedPhysicalInputNames(forElementAlias: String) -> Set&lt;String>

Returns the physical input elements to which the user remaps the given input element.

static let GCControllerUserCustomizationsDidChange: NSNotification.Name

A notification that posts when the user customizes the button mappings or other settings of a controller.

