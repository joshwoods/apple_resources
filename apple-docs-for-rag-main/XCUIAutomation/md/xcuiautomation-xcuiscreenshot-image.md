

- XCUIAutomation
- XCUIScreenshot
-  image 

Instance Property

# image

A representation of the screenshot as a platform-native image object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

**macOS**

``` source
@NSCopying @MainActor
var image: NSImage { get }
```

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
@NSCopying @MainActor
var image: UIImage { get }
```

## See Also

### Screenshot representations

var pngRepresentation: Data

A representation of the screenshot as PNG image data.

