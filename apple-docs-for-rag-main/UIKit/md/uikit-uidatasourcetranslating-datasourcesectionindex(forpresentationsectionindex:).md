

- UIKit
- UIDataSourceTranslating
-  dataSourceSectionIndex(forPresentationSectionIndex:) 

Instance Method

# dataSourceSectionIndex(forPresentationSectionIndex:)

Translates a section index in your presented layout to the equivalent section index in your data source object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func dataSourceSectionIndex(forPresentationSectionIndex presentationSectionIndex: Int) -> Int
```

**Required**

## Parameters 

`presentationSectionIndex`  

The index path of a section in your presentation layer.

## Return Value

The index path of the same section in the data source object, or `nil` if the section is no longer in the data source.

## See Also

### Managing section positions

func presentationSectionIndex(forDataSourceSectionIndex: Int) -> Int

Translates a section index in your data source object to the equivalent section index in your presented layout.

**Required**

