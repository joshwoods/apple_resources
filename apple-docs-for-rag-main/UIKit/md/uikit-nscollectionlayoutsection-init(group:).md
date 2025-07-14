

- UIKit
- NSCollectionLayoutSection
-  init(group:) 

Initializer

# init(group:)

Creates a section containing the specified group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(group: NSCollectionLayoutGroup)
```

## See Also

### Creating a section

static func list(using: UICollectionLayoutListConfiguration, layoutEnvironment: any NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection

Creates a list section with the specified list configuration and layout environment.

class func orthogonalLayoutSectionForMediaItems() -> NSCollectionLayoutSection

Creates an orthogonally scrolling section with system default spacing.

