

- AppKit
- NSCollectionViewSectionHeaderView
-  sectionCollapseButton 

Instance Property

# sectionCollapseButton

A control that lets users collapse and open a collection view section.

macOS 10.12+

``` source
@MainActor @IBOutlet
weak optional var sectionCollapseButton: NSButton? { get set }
```

## Discussion

For the best user experience, set this property to the button that lets users control the collapsing of a section so that the collection view can show and hide the button appropriately, based on whether the section’s items can be displayed in the available space. The collection view uses its toggleSectionCollapse(_:) property to access this button.

