

- Contacts UI
- CNContactViewController
-  highlightProperty(withKey:identifier:) 

Instance Method

# highlightProperty(withKey:identifier:)

Highlights the property of the contact being displayed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func highlightProperty(
    withKey key: String,
    identifier: String?
)
```

## Parameters 

`key`  

Key of the property to highlight.

`identifier`  

`property` is a multivalue property, the value to highlight.

## Discussion

When a single value property key is specified, identifier will be ignored.

