

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityFilename(\_:) 

Instance Method

# setAccessibilityFilename(\_:)

Sets the filename for the file that the accessibility element represents.

macOS 10.10+

``` source
func setAccessibilityFilename(_ accessibilityFilename: String?)
```

**Required**

## See Also

### Managing Documents and Editing

func accessibilityDocument() -> String?

Returns the URL for the file that the accessibility element represents.

**Required**

func setAccessibilityDocument(String?)

Sets the URL for the file that the accessibility element represents.

**Required**

func isAccessibilityEdited() -> Bool

Returns a Boolean value that indicates whether the accessibility element is in an edited state.

**Required**

func setAccessibilityEdited(Bool)

Sets a Boolean value that indicates whether the accessibility element is in an edited state.

**Required**

func accessibilityFilename() -> String?

Returns the filename for the file that the accessibility element represents.

**Required**

