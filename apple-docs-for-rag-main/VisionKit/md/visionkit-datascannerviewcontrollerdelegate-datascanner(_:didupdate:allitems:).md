

- VisionKit
- DataScannerViewControllerDelegate
-  dataScanner(\_:didUpdate:allItems:) 

Instance Method

# dataScanner(\_:didUpdate:allItems:)

Responds when the data scanner updates the geometry of an item it recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
func dataScanner(
    _ dataScanner: DataScannerViewController,
    didUpdate updatedItems: [RecognizedItem],
    allItems: [RecognizedItem]
)
```

**Required** Default implementation provided.

## Parameters 

`dataScanner`  

The data scanner that recognizes the item.

`updatedItems`  

The items with geometry that the data scanner changes.

`allItems`  

The current items that the data scanner tracks. Text items appear in the reading order of the language and region.

## Mentioned in 

Scanning data with the camera

## Discussion

To identify an item in the `updatedItems` and `allItems` parameters, use the item’s `id` property.

## Default Implementations

### DataScannerViewControllerDelegate Implementations

func dataScanner(DataScannerViewController, didUpdate: [RecognizedItem], allItems: [RecognizedItem])

A default, blank implementation for when the data scanner updates the geometry of an item it recognizes.

## See Also

### Customizing highlighting

func dataScanner(DataScannerViewController, didAdd: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner starts recognizing an item.

**Required** Default implementation provided.

func dataScanner(DataScannerViewController, didRemove: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner stops recognizing an item.

**Required** Default implementation provided.

