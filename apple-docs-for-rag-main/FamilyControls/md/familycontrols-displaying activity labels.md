

- FamilyControls
-  Displaying Activity Labels 

API Collection

# Displaying Activity Labels

Provide users with a read-only, visual representation of an application, category, or web domain.

## Overview

To display an application, category, or web domain, choose an ApplicationToken, ActivityCategoryToken, or WebDomainToken that represents an item selected by the user. For example, you can access these tokens from the FamilyActivitySelection bound to a FamilyActivityPicker view.

Use one of these tokens to create a Label instance by passing the token to its initializer. Display the activity item like any SwiftUI view.

```
struct ExampleView: View {
    @State var selection = FamilyActivitySelection()

    var body: some View {
        VStack {
            FamilyActivityPicker(selection: $selection)
            if let applicationToken = selection.applicationTokens.first {
                Label(applicationToken)
            }
        }
    }
}
```

## Topics

### Label Constraints

struct FamilyActivityTitleView

A type-erased view representing the title of the family activity.

struct FamilyActivityIconView

A type-erased view representing the icon of the family activity.

