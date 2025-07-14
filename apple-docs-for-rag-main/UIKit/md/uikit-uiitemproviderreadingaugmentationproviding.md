

- UIKit
-  UIItemProviderReadingAugmentationProviding 

Protocol

# UIItemProviderReadingAugmentationProviding

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 10.4+

``` source
protocol UIItemProviderReadingAugmentationProviding
```

## Topics

### Type Properties

static var additionalLeadingReadableTypeIdentifiersForItemProvider: [String]

**Required**

static var additionalTrailingReadableTypeIdentifiersForItemProvider: [String]

**Required**

### Type Methods

static func object(withItemProviderData: Data, typeIdentifier: String, requestedClass: AnyClass) throws -> Any

**Required**

## See Also

### Item providers

Data delivery with drag and drop

Share data between iPad apps during a drag and drop operation using an item provider.

class NSItemProvider

An item provider for conveying data or a file between processes during drag-and-drop or copy-and-paste activities, or from a host app to an app extension.

protocol NSItemProviderReading : NSObjectProtocol

The protocol for implementing a class to allow an item provider to create an instance of the class.

protocol NSItemProviderWriting : NSObjectProtocol

The protocol for implementing a class to allow an item provider to retrieve data from an instance of the class.

protocol UIItemProviderPresentationSizeProviding

protocol UIItemProviderReadingAugmentationDesignating

