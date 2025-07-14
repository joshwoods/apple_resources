

- Core Data
- NSRelationshipDescription
-  deleteRule 

Instance Property

# deleteRule

The rule to apply when you delete the relationship’s owning managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var deleteRule: NSDeleteRule { get set }
```

## Discussion

The default value is NSDeleteRule.nullifyDeleteRule. For possible values, see NSDeleteRule.

## See Also

### Configuring Delete Behavior

enum NSDeleteRule

Constants that determine what happens when you delete a relationship’s owning managed object.

