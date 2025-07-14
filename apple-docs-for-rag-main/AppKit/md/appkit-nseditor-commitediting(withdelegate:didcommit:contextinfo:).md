

- AppKit
- NSEditor
-  commitEditing(withDelegate:didCommit:contextInfo:) 

Instance Method

# commitEditing(withDelegate:didCommit:contextInfo:)

macOS 10.0+

``` source
@MainActor
func commitEditing(
    withDelegate delegate: Any?,
    didCommit didCommitSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

**Required**

## See Also

### Instance Methods

func commitEditing() -> Bool

**Required**

func commitEditingWithoutPresentingError() throws

**Required**

func discardEditing()

**Required**

