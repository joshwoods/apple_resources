

- SwiftUI
-  DisclosureGroupStyleConfiguration 

Structure

# DisclosureGroupStyleConfiguration

The properties of a disclosure group instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct DisclosureGroupStyleConfiguration
```

## Topics

### Configuring the label

let label: DisclosureGroupStyleConfiguration.Label

The label for the disclosure group.

struct Label

A type-erased label of a disclosure group.

### Configuring the content

let content: DisclosureGroupStyleConfiguration.Content

The content of the disclosure group.

struct Content

A type-erased content of a disclosure group.

### Managing disclosure

var isExpanded: Bool

A binding to a Boolean that indicates whether the disclosure group is expanded.

var $isExpanded: Binding&lt;Bool>

## See Also

### Creating custom disclosure group styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a disclosure group.

**Required**

typealias Configuration

The properties of a disclosure group instance.

associatedtype Body : View

A view that represents the body of a disclosure group.

**Required**

