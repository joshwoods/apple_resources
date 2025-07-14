

- AppKit
- NSCollectionViewCompositionalLayout
-  init(sectionProvider:configuration:) 

Initializer

# init(sectionProvider:configuration:)

Creates a compositional layout object with a section provider and an additional configuration.

macOS 10.15+

``` source
@MainActor
init(
    sectionProvider: @escaping NSCollectionViewCompositionalLayoutSectionProvider,
    configuration: NSCollectionViewCompositionalLayoutConfiguration
)
```

## See Also

### Creating a Layout

init(section: NSCollectionLayoutSection)

Creates a compositional layout object with a single section.

init(section: NSCollectionLayoutSection, configuration: NSCollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a single section and an additional configuration.

init(sectionProvider: NSCollectionViewCompositionalLayoutSectionProvider)

Creates a compositional layout object with a section provider to supply the layout’s sections.

