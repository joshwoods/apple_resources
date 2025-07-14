

- XCUIAutomation
- XCUIElement
-  children(matching:) 

Instance Method

# children(matching:)

Returns a query for all direct children of the element matching the type you specify.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func children(matching type: XCUIElement.ElementType) -> XCUIElementQuery
```

## See Also

### Querying descendant elements

func descendants(matching: XCUIElement.ElementType) -> XCUIElementQuery

Returns a query for all descendants of the element matching the type you specify.

