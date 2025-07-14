

- UIKit
- UIMenuBuilder
-  system 

Instance Property

# system

The menu system that the menu builder modifies.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var system: UIMenuSystem { get }
```

**Required**

## Discussion

Always check the system property to determine which menu system the builder is modifying before you add and remove menus. For example, when you want to modify the main menu bar, check system for main.

```
override func buildMenu(with builder: UIMenuBuilder) {
    super.buildMenu(with: builder)

    // Ensure that the builder is modifying the menu bar system.
    guard builder.system == UIMenuSystem.main else { return }

    let refreshCommand = UICommand(title: "Refresh", action: #selector(refreshData(_:)))
    let refreshMenu = UIMenu(title: "", options: .displayInline, children: [refreshCommand])

    // Insert the menu into the File menu before the Close menu.
    builder.insertSibling(refreshMenu, beforeMenu: .close)
}
```

## See Also

### Getting menu systems and elements

func menu(for: UIMenu.Identifier) -> UIMenu?

Gets the menu for the specified menu identifier.

**Required**

func action(for: UIAction.Identifier) -> UIAction?

Gets the action for the specified action identifier.

**Required**

func command(for: Selector, propertyList: Any?) -> UICommand?

Gets the command for the specified selector and property list.

