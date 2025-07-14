

- XCUIAutomation
-  XCUIElementQuery 

Class

# XCUIElementQuery

An object that defines the search criteria a test uses to identify UI elements.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class XCUIElementQuery
```

## Mentioned in 

Recording UI automation for testing

## Discussion

Use element queries to find UI elements in your app that you interact with in the tests, to test for the presence of expected elements, or to discover elements to test their values.

For example, this test uses an element query to find the “Add Book” button, and after clicking the button, checks that there’s one button in an outline view cell titled “Untitled Book”. If the test can’t find the “Add Book” button, or there isn’t one “Untitled Book” cell, then the test fails.

```
@MainActor
func testClickingAddCreatesAnUntitledBook() throws {
    let app = XCUIApplication()
    app.launch()
    let list = app.windows["Reading Journal"]
    list.toolbars.children(matching: .button)["Add Book"].click()
    XCTAssertEqual(list.outlines["Sidebar"].cells.containing(.button, identifier:"Untitled Book").count, 1)
}
```

## Topics

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

func matching(XCUIElement.ElementType, identifier: String?) -> XCUIElementQuery

Returns a new query that matches elements of the requested type and have an identifying property that matches a provided identifier.

### Accessing matched elements

var allElementsBoundByAccessibilityElement: [XCUIElement]

Immediately evaluates the query and returns an array of elements bound to the resulting accessibility elements.

var allElementsBoundByIndex: [XCUIElement]

Immediately evaluates the query and returns an array of elements bound by the index of each result.

var count: Int

Evaluates the query and returns the number of elements that match.

var element: XCUIElement

The query’s single matching element.

func element(boundBy: Int) -> XCUIElement

Uses an index into the query’s results to determine which underlying accessibility element to use.

func element(matching: NSPredicate) -> XCUIElement

Matches the predicate.

func element(matching: XCUIElement.ElementType, identifier: String?) -> XCUIElement

Matches the provided element type and identifier.

subscript(String) -> XCUIElement

Returns a descendant element that matches a provided identifier.

func element(at: Int) -> XCUIElement

Returns an element that resolves to the index into the query’s result set.

Deprecated

### Debugging element queries

var debugDescription: String

Provides debugging information about the query.

### Identifying window buttons

let XCUIIdentifierCloseWindow: String

The identifier for a window’s close button.

let XCUIIdentifierFullScreenWindow: String

The identifier for a window’s full-screen button.

let XCUIIdentifierMinimizeWindow: String

The identifier for a window’s minimize button.

let XCUIIdentifierZoomWindow: String

The identifier for a window’s zoom button.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- XCUIElementTypeQueryProvider

## See Also

### UI element queries

protocol XCUIElementTypeQueryProvider

A type that provides ready-made queries for locating descendant UI elements.

