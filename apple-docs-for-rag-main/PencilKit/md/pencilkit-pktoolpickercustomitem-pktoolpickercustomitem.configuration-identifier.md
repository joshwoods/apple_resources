

- PencilKit
- PKToolPickerCustomItem
- PKToolPickerCustomItem.Configuration
-  identifier 

Instance Property

# identifier

A string that uniquely identifies the tool in the picker.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
var identifier: String
```

## Discussion

For example, you might use the name `com.example.example-company.custom-tool`. If you use multiple tool items with the same identifier to create the picker, the picker only shows the first instance of that item.

## See Also

### Identifying the custom tool

var name: String

A short string to show as the name of the tool in the UI.

