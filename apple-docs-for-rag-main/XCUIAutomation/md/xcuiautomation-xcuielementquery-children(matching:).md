

- XCUIAutomation
- XCUIElementQuery
-  children(matching:) 

Instance Method

# children(matching:)

Returns a new query that matches all direct children of the requested type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func children(matching type: XCUIElement.ElementType) -> XCUIElementQuery
```

## Parameters 

`type`  

The element type to match.

## Return Value

A new query that defines a search that extends the search criteria of the receiver. The new search finds all direct children of elements that match the original search and are of the requested type. For a list of the types, see XCUIElement.ElementType.

## Discussion

If you need to match all descendants including elements that aren’t direct child elements, use the descendants(matching:) method.

## See Also

### Creating new queries

func descendants(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all descendants of the requested type.

func containing(NSPredicate) -> XCUIElementQuery

Returns a new query that matches elements containing a descendant that meets the logical conditions of the provided predicate.

func containing(XCUIElement.ElementType, identifier: String?) -> XCUIElementQuery

Returns a new query that matches elements that contain a descendant of the requested type and an identifying property that matches a provided identifier.

func matching(identifier: String) -> XCUIElementQuery

Returns a new query that matches elements that have an identifying property that matches a provided identifier.

func matching(NSPredicate) -> XCUIElementQuery

Returns a new query that matches elements that meet the logical conditions of the provided predicate.

func matching(XCUIElement.ElementType, identifier: String?) -> XCUIElementQuery

Returns a new query that matches elements of the requested type and have an identifying property that matches a provided identifier.

