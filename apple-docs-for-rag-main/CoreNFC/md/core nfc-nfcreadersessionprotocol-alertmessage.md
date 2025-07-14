

- Core NFC
- NFCReaderSessionProtocol
-  alertMessage 

Instance Property

# alertMessage

A custom description that helps users understand how they can use NFC reader mode in your app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var alertMessage: String { get set }
```

**Required**

## Discussion

Before you call begin(), use this property to supply a string that provides more context about how your app uses NFC reader mode. For example, you might tell users “Hold your iPhone near the item to learn more about it.” When tag scanning begins, your text is displayed to users in an alert. Note that the alertMessage string is different from the purpose string you supply for the NFCReaderUsageDescription key in your `Info.plist` file.

If you configure your NFC NDEF reader session to read multiple tags, you can update alertMessage to display different information after each tag is read (you can update this string in any thread context while the reader session remains valid).

## See Also

### Managing a Reader Session

func begin()

Starts the reader session.

**Required**

func invalidate()

Closes the reader session, which prevents it from being reused.

**Required**

func invalidate(errorMessage: String)

Closes the reader session and displays an error message to the user.

**Required**

func begin()

Starts the reader session.

**Required**

func invalidate()

Closes the reader session, which prevents it from being reused.

**Required**

func invalidate(errorMessage: String)

Closes the reader session and displays an error message to the user.

**Required**

