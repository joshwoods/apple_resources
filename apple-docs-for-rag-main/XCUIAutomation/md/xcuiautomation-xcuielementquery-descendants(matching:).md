

- XCUIAutomation
- XCUIElementQuery
-  descendants(matching:) 

Instance Method

# descendants(matching:)

Returns a new query that matches all descendants of the requested type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func descendants(matching type: XCUIElement.ElementType) -> XCUIElementQuery
```

## Parameters 

`type`  

The element type to match.

## Return Value

A new query that defines a search that extends the search criteria of the receiver. The new search finds all decendant of elements that match the original search and are of the requested type. For a list of the types, see XCUIElement.ElementType.

## Discussion

Because XCUIElementQuery conforms to the XCUIElementTypeQueryProvider protocol, you can use the protocol’s properties as shorthand for calling descendants(matching:) for different element types. For example, rather than calling `query.descendants(matching: .button)`, you can use the buttons property from the protocol to retrieve `query.buttons`.

## See Also

### Creating new queries

func children(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all direct children of the requested type.

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

