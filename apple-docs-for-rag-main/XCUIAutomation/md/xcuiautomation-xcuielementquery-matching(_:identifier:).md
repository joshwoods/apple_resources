

- XCUIAutomation
- XCUIElementQuery
-  matching(\_:identifier:) 

Instance Method

# matching(\_:identifier:)

Returns a new query that matches elements of the requested type and have an identifying property that matches a provided identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func matching(
    _ elementType: XCUIElement.ElementType,
    identifier: String?
) -> XCUIElementQuery
```

## Parameters 

`elementType`  

The element type to match.

`identifier`  

An optional string to match against any one of each element’s identifying properties: identifier, title, label, value, or placeholderValue.

## Return Value

A new query that defines a search that extends the search criteria of the receiver. The new search matches elements that match the original search of the requested type that have an identifying property matching a provided identifier. For the list of the types, see XCUIElement.ElementType.

## See Also

### Creating new queries

func children(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all direct children of the requested type.

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

