

- Uniform Type Identifiers
- UTType
-  localizedDescription 

Instance Property

# localizedDescription

A localized description of the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var localizedDescription: String? { get }
```

## Discussion

If the type doesn’t provide a description, the system searches its supertypes. A dynamic type doesn’t have localized description, even if its supertypes do.

