

- CarPlay
- CPListTemplate
- CPListSection
- CPListItem
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated Methods

init(text: String?, detailText: String?, image: UIImage?, showsDisclosureIndicator: Bool)

Creates a list item with primary text, secondary text, an image, and a disclosure indicator.

Deprecated

### Deprecated Properties

var showsDisclosureIndicator: Bool

A Boolean value that indicates whether the list item cell shows a disclosure indicator on its trailing edge.

Deprecated

var showsExplicitLabel: Bool

A Boolean value that determines whether the list item displays its explicit content indicator.

Deprecated

func setRootTemplate(CPTemplate, animated: Bool)

Sets the root template, starting a new stack for the template navigation hierarchy.

Deprecated

func pushTemplate(CPTemplate, animated: Bool)

Pushes a template onto the navigation stack and updates the CarPlay display.

Deprecated

func popTemplate(animated: Bool)

Pops the top template from the navigation stack and updates the CarPlay display.

Deprecated

func popToRootTemplate(animated: Bool)

Pops all templates on the stack—except the root template—and updates the CarPlay display.

Deprecated

func pop(to: CPTemplate, animated: Bool)

Pops templates until the specified template is at the top of the navigation stack.

Deprecated

func presentTemplate(CPTemplate, animated: Bool)

Presents a template modally.

Deprecated

func dismissTemplate(animated: Bool)

Dismisses the template that the interface controller is displaying modally.

Deprecated

