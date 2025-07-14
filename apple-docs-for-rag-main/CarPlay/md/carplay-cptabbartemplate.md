

- CarPlay
-  CPTabBarTemplate 

Class

# CPTabBarTemplate

A container template that displays and manages other templates, presenting them as tabs.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPTabBarTemplate
```

## Overview

`CPTabBarTemplate` is a container template that displays a collection of other templates, where each template occupies a single tab in the tab bar. At runtime, use maximumTabCount to determine the maximum number of tabs that your tab bar can display.

When creating an instance of `CPTabBarTemplate`, provide an array of templates for the tab bar to display. CarPlay treats the array’s templates as root templates, each with its own navigation hierarchy. When a tab bar template is the rootTemplate of your app’s interface controller and you use the controller to add and remove templates, CarPlay applies those changes to the selected tab’s navigation hierarchy.

Note

You can’t add a tab bar template to an existing navigation hierarchy, or present one modally. Instead, use setRootTemplate(_:animated:completion:) to set the tab bar as your app’s root template.

Use a transactional approach when making changes to the tab bar. Retrieve the current set of templates using the templates property. Add, remove, reorder, or make appearance changes to one or more of the array’s templates. For example, use the tabTitle property to update a template’s tab title, or set showsTabBadge to `true` to add an indicator to a template’s tab. Then call the updateTemplates(_:) method and pass it the updated array. CarPlay commits those changes and updates the tab bar.

When the user selects a tab, the template calls the tabBarTemplate(_:didSelect:) method on its delegate, which is an object you provide that conforms to the CPTabBarTemplateDelegate protocol.

## Topics

### Creating a Tab Bar Template

init(templates: [CPTemplate])

Creates a tab bar template that displays the provided root templates as tabs.

### Managing Tab Bar Interactions

var delegate: (any CPTabBarTemplateDelegate)?

The object that acts as the template’s delegate.

protocol CPTabBarTemplateDelegate

The methods an object implements to act as the delegate for a tab bar template.

### Managing the Templates

var templates: [CPTemplate]

The tab bar’s templates.

func updateTemplates([CPTemplate])

Adds, removes, reorders, or updates the tab bar’s templates.

class var maximumTabCount: Int

The maximum number of tabs that the template can display.

### Getting the Selected Template

var selectedTemplate: CPTemplate?

The currently selected template in the tab bar.

### Instance Methods

func select(CPTemplate)

func selectTemplate(at: Int)

## Relationships

### Inherits From

- CPTemplate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### General Purpose Templates

class CPListTemplate

A template that displays and manages a list of items.

class CPGridTemplate

A template that displays and manages a grid of items.

class CPTemplate

An abstract base class for interface templates.

protocol CPBarButtonProviding

The methods that templates use to provide buttons for the navigation bar.

