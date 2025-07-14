

- AppKit
- NSFontCollection
-  rename(fromName:visibility:toName:) 

Type Method

# rename(fromName:visibility:toName:)

Renames the font collection with the specified name and visibility to the second name specified.

macOS 10.7+

``` source
class func rename(
    fromName oldName: NSFontCollection.Name,
    visibility: NSFontCollection.Visibility,
    toName newName: NSFontCollection.Name
) throws
```

## Parameters 

`oldName`  

The collection to rename.

`visibility`  

The visibility of the collection to rename.

`newName`  

The new name to give to the collection.

## Discussion

Named collections are shown by user interfaces such as the Font panel. When you change the collection, you must show it again to see the changes reflected on disk or in the Font panel.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Naming the Font Collection

class func show(NSFontCollection, withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Make the given font collection visible by giving it a name.

class func hide(withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Remove from view the named font collection with the specified visibility.

class var allFontCollectionNames: [NSFontCollection.Name]

Returns all named collections visible to this process.

struct Name

The constants represent the standard mutable collection names—these names are included in the list of allFontCollectionNames–they have special meaning to the Cocoa font system and should not be hidden or renamed.

struct Visibility

Constants that specify the visibility of font collections.

