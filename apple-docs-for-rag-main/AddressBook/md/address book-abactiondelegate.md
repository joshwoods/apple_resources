

- Address Book
-  ABActionDelegate 

# ABActionDelegate

Implement an Address Book action plug-in to support the display of rollover menus on top of custom items.

## Overview

The `ABActionDelegate` informal protocol allows you to populate the rollover menus of Address Book with custom items. You do this by implementing an Address Book action plug-in. The plug-in’s Bundle must implement actionProperty(), title(for:identifier:), and performAction(for:identifier:).

Each action plug-in can implement only one action. Actions can only apply to items with labels. An action can display a simple window inside the Address Book application; if your action actions needs to do anything else, it should launch your own application to perform the action.

Use Xcode to create Address Book action plug-ins. Place action plug-ins in `~/Library/Address Book Plug-Ins` or `/Library/Address Book Plug-Ins`, depending on the scope you want for the action.

## Topics

### Performing actions

func performAction(for person: ABPerson!, identifier: String!)

Sent to the delegate to perform the action.

### Querying

func actionProperty() -> String!

Sent to the delegate to request the property the action applies to.

func shouldEnableAction(for person: ABPerson!, identifier: String!) -> Bool

Sent to the delegate to determine whether the action should be enabled.

func title(for person: ABPerson!, identifier: String!) -> String!

Sent to the delegate to request the title of the menu item for the action.

