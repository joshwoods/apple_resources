

- VisionKit
- DataScannerViewControllerDelegate
-  dataScanner(\_:didRemove:allItems:) 

Instance Method

# dataScanner(\_:didRemove:allItems:)

Responds when the data scanner stops recognizing an item.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
func dataScanner(
    _ dataScanner: DataScannerViewController,
    didRemove removedItems: [RecognizedItem],
    allItems: [RecognizedItem]
)
```

**Required** Default implementation provided.

## Parameters 

`dataScanner`  

The data scanner that recognizes the item.

`removedItems`  

The items that the data scanner removes from the recognizedItems property.

`allItems`  

The current items that the data scanner tracks. Text items appear in the reading order of the language and region.

## Mentioned in 

Scanning data with the camera

## Discussion

To identify an item in the `removedItems` and `allItems` parameters, use the item’s `id` property.

## Default Implementations

### DataScannerViewControllerDelegate Implementations

func dataScanner(DataScannerViewController, didRemove: [RecognizedItem], allItems: [RecognizedItem])

A default, blank implementation for when the data scanner stops recognizing an item.

## See Also

### Customizing highlighting

func dataScanner(DataScannerViewController, didAdd: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner starts recognizing an item.

**Required** Default implementation provided.

func dataScanner(DataScannerViewController, didUpdate: [RecognizedItem], allItems: [RecognizedItem])

Responds when the data scanner updates the geometry of an item it recognizes.

**Required** Default implementation provided.

