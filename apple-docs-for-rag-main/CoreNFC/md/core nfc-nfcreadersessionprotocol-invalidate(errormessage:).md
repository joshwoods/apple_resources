

- Core NFC
- NFCReaderSessionProtocol
-  invalidate(errorMessage:) 

Instance Method

# invalidate(errorMessage:)

Closes the reader session and displays an error message to the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func invalidate(errorMessage: String)
```

**Required**

## Parameters 

`errorMessage`  

The error message to display.

## Discussion

Use this method to end the reader session and display a message to the user when an error condition occurs after the app successfully reads a tag. This type of error can occur if, for example, the app reads data from an NFC tag, but determines that the data has expired and discards it. The app then calls invalidate(errorMessage:) to end the reader session, and to let the user know why it discarded the data.

Note

After invalidating a reader session, you cannot use it to scan and detect other tags.

## See Also

### Managing a Reader Session

func begin()

Starts the reader session.

**Required**

func invalidate()

Closes the reader session, which prevents it from being reused.

**Required**

var alertMessage: String

A custom description that helps users understand how they can use NFC reader mode in your app.

**Required**

func begin()

Starts the reader session.

**Required**

func invalidate()

Closes the reader session, which prevents it from being reused.

**Required**

var alertMessage: String

A custom description that helps users understand how they can use NFC reader mode in your app.

**Required**

