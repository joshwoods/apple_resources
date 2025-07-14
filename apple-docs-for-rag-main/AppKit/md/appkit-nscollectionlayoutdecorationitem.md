

- AppKit
-  NSCollectionLayoutDecorationItem 

Class

# NSCollectionLayoutDecorationItem

An object used to add a background to a section of a collection view.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutDecorationItem
```

## Overview

Each type of decoration item must have a unique element kind. Consider tracking these strings together in a way that makes it straightforward to identify each element, for example:

- Swift
- Objective-C

```
struct ElementKind {
    static let badge = "badge-element-kind"
    static let background = "background-element-kind"
    static let sectionHeader = "section-header-element-kind"
    static let sectionFooter = "section-footer-element-kind"
    static let layoutHeader = "layout-header-element-kind"
    static let layoutFooter = "layout-footer-element-kind"
}
```

```
NSString* const ELEMENT_KIND_BADGE = @"badge-elemn’s-kind";
NSString* const ELEMENT_KIND_BACKGROUND = @"background-element-kind";
NSString* const ELEMENT_KIND_SECTION_HEADER = @"section-header-element-kind";
NSString* const ELEMENT_KIND_SECTION_FOOTER = @"section-footer-element-kind";
NSString* const ELEMENT_KIND_LAYOUT_HEADER = @"layout-header-element-kind";
NSString* const ELEMENT_KIND_LAYOUT_FOOTER = @"layout-footer-element-kind";
```

Add a background to a section by setting that section’s decorationItems property:

- Swift
- Objective-C

```
let sectionBackground = NSCollectionLayoutDecorationItem.background(
        elementKind: ElementKind.background)

section.decorationItems = [sectionBackground]

let layout = UICollectionViewCompositionalLayout(section: section)
layout.register(
    SectionBackgroundDecorationView.self,
    forDecorationViewOfKind: ElementKind.background)
return layout
```

```
NSCollectionLayoutDecorationItem *sectionBackground = [NSCollectionLayoutDecorationItem backgroundDecorationItemWithElementKind: ELEMENT_KIND_BACKGROUND];

[section setDecorationItems: @[sectionBackground]];

UICollectionViewCompositionalLayout *layout = [[UICollectionViewCompositionalLayout alloc] initWithSection: section];
[layout registerClass: [SectionBackgroundDecorationView class] forDecorationViewOfKind: ELEMENT_KIND_BACKGROUND];
return layout;
```

## Topics

### Creating a background

class func background(elementKind: String) -> Self

Creates a section background with a string to identify the element kind.

### Getting the element kind

var elementKind: String

A string that identifies the type of decoration item.

### Specifying stacking order

var zIndex: Int

The vertical stacking order of the decoration item in relation to other items in the section.

## Relationships

### Inherits From

- NSCollectionLayoutItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Appearance

class NSCollectionLayoutBoundarySupplementaryItem

An object used to add headers or footers to a collection view.

class NSCollectionLayoutSupplementaryItem

An object used to add an extra visual decoration to an item in a collection view.

class NSCollectionLayoutAnchor

An object that defines how to attach a supplementary item to an item in a collection view.

