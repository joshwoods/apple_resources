

- Game Controller
- GCDevice
-  Product category constants 

API Collection

# Product category constants

## Topics

### Game controller categories

let GCProductCategoryDualSense: String

The DualSense product category.

let GCProductCategoryDualShock4: String

The DualShock 4 product category.

let GCProductCategoryMFi: String

The MFi product category.

let GCProductCategoryXboxOne: String

The Xbox product category.

let GCProductCategoryArcadeStick: String

The arcade stick product category.

let GCProductCategoryHID: String

The category for products that support the human interface device (HID) protocol.

### Apple TV remote categories

let GCProductCategorySiriRemote1stGen: String

The first-generation Siri Remote or first-generation Apple TV Remote product category.

let GCProductCategorySiriRemote2ndGen: String

The second-generation Siri Remote or second-generation Apple TV Remote product category.

let GCProductCategoryControlCenterRemote: String

The virtual remote in the Control Center on iOS and tvOS devices for controlling the Apple TV.

let GCProductCategoryUniversalElectronicsRemote: String

The product category for a Universal Electronics remote that works with Apple TV.

let GCProductCategoryCoalescedRemote: String

The Apple TV Remote product category for physical and virtual remotes that Game Center combines into a single device.

### Mouse and keyboard categories

let GCProductCategoryMouse: String

The mouse product category.

let GCProductCategoryKeyboard: String

The keyboard product category.

## See Also

### Getting device information

var vendorName: String?

The manufacturer-provided name for the device, or the user’s name for the device.

**Required**

var productCategory: String

The product category that identifies the type of controller.

**Required**

