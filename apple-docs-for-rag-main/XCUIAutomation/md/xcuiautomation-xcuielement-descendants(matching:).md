

- XCUIAutomation
- XCUIElement
-  descendants(matching:) 

Instance Method

# descendants(matching:)

Returns a query for all descendants of the element matching the type you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func descendants(matching type: XCUIElement.ElementType) -> XCUIElementQuery
```

## Discussion

Because XCUIElement conforms to the XCUIElementTypeQueryProvider protocol, you can use the protocol’s properties as shorthand for calling descendants(matching:) for different element types. For example, rather than calling `table.descendants(matching: .cell)`, you can use the cells property from the protocol to retrieve `table.cells`.

## See Also

### Querying descendant elements

func children(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a query for all direct children of the element matching the type you specify.

