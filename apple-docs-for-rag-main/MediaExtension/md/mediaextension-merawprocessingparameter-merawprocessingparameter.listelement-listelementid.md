

- MediaExtension
- MERAWProcessingParameter
- MERAWProcessingParameter.ListElement
-  listElementID 

Instance Property

# listElementID

A unique number in the list which represents this list option.

macOS 15.0+

``` source
var listElementID: Int { get }
```

## Discussion

The set of elements in the list may change depending on other configuration parameters, so while the index of an element in this list may change, this ID never changes and is used to report list element selection.

