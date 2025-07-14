

- AppKit
-  NSCollectionViewCompositionalLayoutSectionProvider 

Type Alias

# NSCollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

macOS

``` source
typealias NSCollectionViewCompositionalLayoutSectionProvider = (Int, any NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection?
```

## Discussion

You use a section provider to create a compositional layout (NSCollectionViewCompositionalLayout) that has multiple sections with different layouts. The section provider keeps track of the index of the section that it’s currently creating, so you can configure each section differently.

For example, the following code shows a section provider that creates a two-column layout in the first section, and a four-column layout in each section after the first section.

```
func createPerSectionLayout() -> NSCollectionViewLayout {
    let layout = NSCollectionViewCompositionalLayout { (sectionIndex: Int,
        layoutEnvironment: NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection? in

        let columns = sectionIndex == 0 ? 2 : 4

        let itemSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(1.0),
                                             heightDimension: .fractionalHeight(1.0))
        let item = NSCollectionLayoutItem(layoutSize: itemSize)

        let groupSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(1.0),
                                              heightDimension: .absolute(44))
        let group = NSCollectionLayoutGroup.horizontal(layoutSize: groupSize,
                                                          subitem: item,
                                                            count: columns)

        let section = NSCollectionLayoutSection(group: group)
        return section
    }
    return layout
}
```

A section provider is also invoked in response to system events such as changes in system font size. You can use this opportunity to adapt the layout to different layout environments by inspecting information about the current layout environment (NSCollectionLayoutEnvironment) and using that information to configure each section.

For example, the following code shows a section provider that creates a two-column layout when the width of the section’s container is less than 800 points, and a four-column layout otherwise.

```
func createAdaptiveLayout() -> NSCollectionViewLayout {
    let layout = NSCollectionViewCompositionalLayout { (sectionIndex: Int,
        layoutEnvironment: NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection in

        let columns = layoutEnvironment.container.effectiveContentSize.width 

## See Also

### Layouts

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

class NSCollectionViewFlowLayout

A layout that organizes items into a flexible and configurable arrangement.

protocol NSCollectionViewDelegateFlowLayout

A set of methods that a delegate implements to provide layout information to a flow layout object in a collection view.

class NSCollectionViewGridLayout

A layout that displays a single section of items in a row and column grid.

class NSCollectionViewTransitionLayout

An object that implements custom behaviors when changing from one layout to another in a collection view.

class NSCollectionViewLayoutAttributes

An object that contains layout-related attributes for an element in a collection view.

class NSCollectionViewLayout

An abstract base class that you subclass and use to generate layout information for a collection view.

class NSCollectionViewCompositionalLayout

A layout object that lets you combine items in highly adaptive and flexible visual arrangements.

class NSCollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

enum NSCollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

