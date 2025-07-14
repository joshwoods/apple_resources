

- Game Controller
-  GCProductCategoryCoalescedRemote 

Global Variable

# GCProductCategoryCoalescedRemote

The Apple TV Remote product category for physical and virtual remotes that Game Center combines into a single device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
let GCProductCategoryCoalescedRemote: String
```

## Discussion

Game Controller merges the physical Apple TV Remote with the virtual Apple TV Remote app into one GCDevice object by default. To disable this behavior, or if you fully support the second-generation Siri Remote, set the GCSupportsMultipleMicroGamepads key to `YES` in the information property list.

## See Also

### Apple TV remote categories

let GCProductCategorySiriRemote1stGen: String

The first-generation Siri Remote or first-generation Apple TV Remote product category.

let GCProductCategorySiriRemote2ndGen: String

The second-generation Siri Remote or second-generation Apple TV Remote product category.

let GCProductCategoryControlCenterRemote: String

The virtual remote in the Control Center on iOS and tvOS devices for controlling the Apple TV.

let GCProductCategoryUniversalElectronicsRemote: String

The product category for a Universal Electronics remote that works with Apple TV.

