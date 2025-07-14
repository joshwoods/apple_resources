

- UIKit
- UIDataSourceTranslating
-  presentationSectionIndex(forDataSourceSectionIndex:) 

Instance Method

# presentationSectionIndex(forDataSourceSectionIndex:)

Translates a section index in your data source object to the equivalent section index in your presented layout.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func presentationSectionIndex(forDataSourceSectionIndex dataSourceSectionIndex: Int) -> Int
```

**Required**

## Parameters 

`dataSourceSectionIndex`  

The index path of a section in the data source object.

## Return Value

The index path of the same section in the presentation layer of your object, or `nil` if the section is not in the presentation layer.

## See Also

### Managing section positions

func dataSourceSectionIndex(forPresentationSectionIndex: Int) -> Int

Translates a section index in your presented layout to the equivalent section index in your data source object.

**Required**

