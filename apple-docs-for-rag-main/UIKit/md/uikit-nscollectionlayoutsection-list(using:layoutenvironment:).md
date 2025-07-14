

- UIKit
- NSCollectionLayoutSection
-  list(using:layoutEnvironment:) 

Type Method

# list(using:layoutEnvironment:)

Creates a list section with the specified list configuration and layout environment.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
static func list(
    using configuration: UICollectionLayoutListConfiguration,
    layoutEnvironment: any NSCollectionLayoutEnvironment
) -> NSCollectionLayoutSection
```

## See Also

### Creating a section

convenience init(group: NSCollectionLayoutGroup)

Creates a section containing the specified group.

class func orthogonalLayoutSectionForMediaItems() -> NSCollectionLayoutSection

Creates an orthogonally scrolling section with system default spacing.

