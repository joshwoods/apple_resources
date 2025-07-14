

- Core NFC
- NFCReaderSessionProtocol
-  invalidate() 

Instance Method

# invalidate()

Closes the reader session, which prevents it from being reused.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func invalidate()
```

**Required**

## See Also

### Managing a Reader Session

func begin()

Starts the reader session.

**Required**

func invalidate(errorMessage: String)

Closes the reader session and displays an error message to the user.

**Required**

var alertMessage: String

A custom description that helps users understand how they can use NFC reader mode in your app.

**Required**

func begin()

Starts the reader session.

**Required**

func invalidate(errorMessage: String)

Closes the reader session and displays an error message to the user.

**Required**

var alertMessage: String

A custom description that helps users understand how they can use NFC reader mode in your app.

**Required**

