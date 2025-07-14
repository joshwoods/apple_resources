

- Foundation
- URL
-  appendPathExtension(\_:) 

Instance Method

# appendPathExtension(\_:)

Appends the specified path extension to self.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func appendPathExtension(_ pathExtension: String)
```

## Parameters 

`pathExtension`  

The extension to append.

## Discussion

If the URL has an empty path, such as `http://www.example.com`, this function does nothing. Certain special characters (for example, Unicode right-to-left marks) can’t be path extensions. If `pathExtension` contains any of those characters, the function returns an unchanged URL.

## See Also

### Adding a path extension

func appendingPathExtension(String) -> URL

Returns a URL by appending the specified path extension to self.

func appendPathExtension(for: UTType)

Appends the preferred path extension for the type you specify.

func appendingPathExtension(for: UTType) -> URL

Returns a URL by appending the preferred path extension for the type you specify to the URL’s last path component.

