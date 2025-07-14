

- SwiftUI
- ForEach
-  init(sections:content:) 

Initializer

# init(sections:content:)

Creates an instance that uniquely identifies and creates views across updates based on the sections of a given view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    sections view: V,
    @ViewBuilder content: @escaping (SectionConfiguration) -> Content
) where Data == ForEachSectionCollection, ID == SectionConfiguration.ID, Content : View, V : View
```

Available when `Data` conforms to `RandomAccessCollection` and `ID` conforms to `Hashable`.

## Parameters 

`view`  

The view to extract the sections of.

`content`  

The view builder that creates views from sections

