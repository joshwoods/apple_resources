

- UIKit
-  UICollectionViewCompositionalLayout 

Class

# UICollectionViewCompositionalLayout

A layout object that lets you combine items in highly adaptive and flexible visual arrangements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UICollectionViewCompositionalLayout
```

## Overview

A compositional layout is a type of collection view layout. It’s designed to be composable, flexible, and fast, letting you build any kind of visual arrangement for your content by combining — or compositing — each smaller component into a full layout.

A compositional layout is composed of one or more sections that break up the layout into distinct visual groupings. Each section is composed of groups of individual items, the smallest unit of data you want to present. A group might lay out its items in a horizontal row, a vertical column, or a custom arrangement.

You combine the components by building up from items into a group, from groups into a section, and finally into a full layout, like in this example of a basic list layout:

- Swift
- Objective-C

```
func createBasicListLayout() -> UICollectionViewLayout { 
    let itemSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(1.0),                                  
                                         heightDimension: .fractionalHeight(1.0))    
    let item = NSCollectionLayoutItem(layoutSize: itemSize)  

    let groupSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(1.0),                                          
                                          heightDimension: .absolute(44))    
    let group = NSCollectionLayoutGroup.horizontal(layoutSize: groupSize,                                                   
                                                     subitems: [item])  

    let section = NSCollectionLayoutSection(group: group)    

    let layout = UICollectionViewCompositionalLayout(section: section)    
    return layout
}
```

```
- (UICollectionViewLayout *)createBasicListLayout {
    NSCollectionLayoutSize *itemSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension fractionalWidthDimension:1.0] heightDimension:[NSCollectionLayoutDimension fractionalHeightDimension:1.0]];

    NSCollectionLayoutItem *item = [NSCollectionLayoutItem itemWithLayoutSize:itemSize];

    NSCollectionLayoutSize *groupSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension fractionalWidthDimension:1.0] heightDimension:[NSCollectionLayoutDimension absoluteDimension:44.0]];

    NSCollectionLayoutGroup *group = [NSCollectionLayoutGroup horizontalGroupWithLayoutSize:groupSize subitems:@[item]];

    NSCollectionLayoutSection *section = [NSCollectionLayoutSection sectionWithGroup:group];

    UICollectionViewCompositionalLayout *layout = [[UICollectionViewCompositionalLayout alloc] initWithSection:section];

    return layout;
}
```

## Topics

### Creating a layout

init(section: NSCollectionLayoutSection)

Creates a compositional layout object with a single section.

init(section: NSCollectionLayoutSection, configuration: UICollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a single section and an additional configuration.

init(sectionProvider: UICollectionViewCompositionalLayoutSectionProvider)

Creates a compositional layout object with a section provider to supply the layout’s sections.

init(sectionProvider: UICollectionViewCompositionalLayoutSectionProvider, configuration: UICollectionViewCompositionalLayoutConfiguration)

Creates a compositional layout object with a section provider and an additional configuration.

### Creating a list layout

static func list(using: UICollectionLayoutListConfiguration) -> UICollectionViewCompositionalLayout

Creates a compositional layout that contains only list sections of the specified configuration.

struct UICollectionLayoutListConfiguration

A configuration for creating a list layout.

### Configuring the layout

var configuration: UICollectionViewCompositionalLayoutConfiguration

The layout’s configuration, such as its scroll direction and section spacing.

## Relationships

### Inherits From

- UICollectionViewLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Essentials

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

