

- UIKit
- UICollectionViewCompositionalLayout
-  init(sectionProvider:) 

Initializer

# init(sectionProvider:)

Creates a compositional layout object with a section provider to supply the layout’s sections.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(sectionProvider: @escaping UICollectionViewCompositionalLayoutSectionProvider)
```

## See Also

### Creating a layout

init(section: NSCollectionLayoutSection)

Creates a compositional layout object with a single section.

init(section: NSCollectionLayoutSection, configuration: UICollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a single section and an additional configuration.

init(sectionProvider: UICollectionViewCompositionalLayoutSectionProvider, configuration: UICollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a section provider and an additional configuration.

