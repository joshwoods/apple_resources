

- AppKit
- NSPredicateEditorRowTemplate
-  templates(withAttributeKeyPaths:in:) 

Type Method

# templates(withAttributeKeyPaths:in:)

Returns an array of predicate templates for the given attribute key paths for a given entity.

macOS 10.5+

``` source
class func templates(
    withAttributeKeyPaths keyPaths: [String],
    in entityDescription: NSEntityDescription
) -> [NSPredicateEditorRowTemplate]
```

## Parameters 

`keyPaths`  

An array of attribute key paths originating at `entityDescription`. The key paths may cross relationships but must terminate in attributes.

`entityDescription`  

A Core Data entity description.

## Return Value

An array of predicate templates for `keyPaths` originating at `entityDescription`.

## Discussion

This method determines which key paths in the entity description can use the same views (that is, share the same attribute type). For each of these groups, it instantiates individual templates via init(leftExpressions:rightExpressions:modifier:operators:options:).

