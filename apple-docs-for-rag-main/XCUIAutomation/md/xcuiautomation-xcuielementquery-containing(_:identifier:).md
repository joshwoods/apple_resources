

- XCUIAutomation
- XCUIElementQuery
-  containing(\_:identifier:) 

Instance Method

# containing(\_:identifier:)

Returns a new query that matches elements that contain a descendant of the requested type and an identifying property that matches a provided identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func containing(
    _ elementType: XCUIElement.ElementType,
    identifier: String?
) -> XCUIElementQuery
```

## Parameters 

`elementType`  

The contained element type to match.

`identifier`  

An optional string to match against the contained element’s identifying properties: identifier, title, label, value, or placeholderValue.

## Return Value

A new query that defines a search that extends the search criteria of the receiver. The new search finds elements that match the original search and contain elements of the requested type that have an identifying property that matches a provided identifier. For the list of the types, see XCUIElement.ElementType.

## See Also

### Creating new queries

func children(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all direct children of the requested type.

func descendants(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all descendants of the requested type.

func containing(NSPredicate) -> XCUIElementQuery

Returns a new query that matches elements containing a descendant that meets the logical conditions of the provided predicate.

func matching(identifier: String) -> XCUIElementQuery

Returns a new query that matches elements that have an identifying property that matches a provided identifier.

func matching(NSPredicate) -> XCUIElementQuery

Returns a new query that matches elements that meet the logical conditions of the provided predicate.

func matching(XCUIElement.ElementType, identifier: String?) -> XCUIElementQuery

Returns a new query that matches elements of the requested type and have an identifying property that matches a provided identifier.

