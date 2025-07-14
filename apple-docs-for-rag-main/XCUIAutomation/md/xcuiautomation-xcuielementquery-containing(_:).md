

- XCUIAutomation
- XCUIElementQuery
-  containing(\_:) 

Instance Method

# containing(\_:)

Returns a new query that matches elements containing a descendant that meets the logical conditions of the provided predicate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func containing(_ predicate: NSPredicate) -> XCUIElementQuery
```

## Parameters 

`predicate`  

The predicate used to evaluate each descendant element.

## Return Value

A new query that defines a search that extends the search criteria of the receiver. The new search finds elements that match the original search and contain elements that meet the logical conditions of the provided predicate.

## Discussion

The predicate evaluates against objects that conform to the XCUIElementAttributes protocol.

Note

Where possible, use NSExpression-based or format-string-based predicates with this method in preference to block-based predicates. This enables the framework to optimize the query’s performance.

## See Also

### Creating new queries

func children(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all direct children of the requested type.

func descendants(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a new query that matches all descendants of the requested type.

func containing(XCUIElement.ElementType, identifier: String?) -> XCUIElementQuery

Returns a new query that matches elements that contain a descendant of the requested type and an identifying property that matches a provided identifier.

func matching(identifier: String) -> XCUIElementQuery

Returns a new query that matches elements that have an identifying property that matches a provided identifier.

func matching(NSPredicate) -> XCUIElementQuery

Returns a new query that matches elements that meet the logical conditions of the provided predicate.

func matching(XCUIElement.ElementType, identifier: String?) -> XCUIElementQuery

Returns a new query that matches elements of the requested type and have an identifying property that matches a provided identifier.

