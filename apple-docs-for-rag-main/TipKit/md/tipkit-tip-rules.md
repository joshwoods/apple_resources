

- TipKit
- Tip
-  rules 

Instance Property

# rules

The rules that determine when a tip is eligible for display. For more information on rules, see Tips.Rule.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@Tips.RuleBuilder var rules: [Self.Rule] { get }
```

**Required**

## Discussion

Use this property to define the rules for when your tips display. If you don’t supply a value, this property returns an empty array of type `Rule`.

## See Also

### Controlling when tips appear

typealias Rule

A condition to meet before displaying a tip.

typealias Event

A repeatable user-defined action.

