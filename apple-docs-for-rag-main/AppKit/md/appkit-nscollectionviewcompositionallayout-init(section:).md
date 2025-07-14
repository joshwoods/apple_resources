

- AppKit
- NSCollectionViewCompositionalLayout
-  init(section:) 

Initializer

# init(section:)

Creates a compositional layout object with a single section.

macOS 10.15+

``` source
@MainActor
init(section: NSCollectionLayoutSection)
```

## See Also

### Creating a Layout

init(section: NSCollectionLayoutSection, configuration: NSCollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a single section and an additional configuration.

init(sectionProvider: NSCollectionViewCompositionalLayoutSectionProvider)

Creates a compositional layout object with a section provider to supply the layout’s sections.

init(sectionProvider: NSCollectionViewCompositionalLayoutSectionProvider, configuration: NSCollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a section provider and an additional configuration.

