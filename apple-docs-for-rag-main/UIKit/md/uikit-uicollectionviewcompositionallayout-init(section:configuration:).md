

- UIKit
- UICollectionViewCompositionalLayout
-  init(section:configuration:) 

Initializer

# init(section:configuration:)

Creates a compositional layout object with a single section and an additional configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(
    section: NSCollectionLayoutSection,
    configuration: UICollectionViewCompositionalLayoutConfiguration
)
```

## See Also

### Creating a layout

init(section: NSCollectionLayoutSection)

Creates a compositional layout object with a single section.

init(sectionProvider: UICollectionViewCompositionalLayoutSectionProvider)

Creates a compositional layout object with a section provider to supply the layout’s sections.

init(sectionProvider: UICollectionViewCompositionalLayoutSectionProvider, configuration: UICollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a section provider and an additional configuration.

