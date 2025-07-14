

- Social
-  SLComposeSheetConfigurationItem 

Class

# SLComposeSheetConfigurationItem

An object that provides additional configuration details to use when configuring a composition interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
class SLComposeSheetConfigurationItem
```

## Overview

The SLComposeSheetConfigurationItem class gives users a way to configure the properties of a post before posting it. For example, you can use these objects to let users choose an account from which to post, an album to which to post, or a location to add to a post.

To provide support for post configurations in your SLComposeServiceViewController view, create as many configuration items as you need, place them in an array, and return the array in your implementation of `configurationItems`. Note that only one configuration item can be displayed at a time.

## Topics

### Creating a Configuration Item

init!()

Returns a configuration item.

### Responding to User Interaction

var tapHandler: SLComposeSheetConfigurationItemTapHandler!

A custom tap handler block that handles user interaction with a configuration item.

typealias SLComposeSheetConfigurationItemTapHandler

The method signature for a configuration item’s tap handler block.

### Specifying Configuration Information

var title: String!

The name of the configuration item stored as a localized string.

var value: String!

The current value or setting of the configuration item.

var valuePending: Bool

A Boolean value that indicates whether the configuration item’s value is ready for display.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring the Post Details

func configurationItems() -> [Any]!

Returns configuration items to display in the compose view.

func reloadConfigurationItems()

Reloads the list of configuration items.

