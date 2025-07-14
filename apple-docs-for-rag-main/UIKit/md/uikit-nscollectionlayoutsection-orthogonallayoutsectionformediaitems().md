

- UIKit
- NSCollectionLayoutSection
-  orthogonalLayoutSectionForMediaItems() 

Type Method

# orthogonalLayoutSectionForMediaItems()

Creates an orthogonally scrolling section with system default spacing.

tvOS 15.0+

``` source
@MainActor
class func orthogonalLayoutSectionForMediaItems() -> NSCollectionLayoutSection
```

## See Also

### Creating a section

convenience init(group: NSCollectionLayoutGroup)

Creates a section containing the specified group.

static func list(using: UICollectionLayoutListConfiguration, layoutEnvironment: any NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection

Creates a list section with the specified list configuration and layout environment.

