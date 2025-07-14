

- Application Services
- UniversalAccess.h
-  UAZoomEnabled() 

Function

# UAZoomEnabled()

Determines if the Universal Access zoom feature is enabled.

macOS 10.4+

``` source
func UAZoomEnabled() -> Bool
```

## Return Value

Returns `true` if the Universal Access zoom feature is on, `false` if the zoom feature is off or if the user has zoomed all the way out.

## See Also

### Miscellaneous

func UAZoomChangeFocus(UnsafePointer&lt;CGRect>!, UnsafePointer&lt;CGRect>!, UAZoomChangeFocusType) -> OSStatus

Tells the Universal Access zoom feature where it should focus.

