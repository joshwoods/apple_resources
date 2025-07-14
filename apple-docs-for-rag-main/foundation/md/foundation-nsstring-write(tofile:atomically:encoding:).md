

- Foundation
- NSString
-  write(toFile:atomically:encoding:) 

Instance Method

# write(toFile:atomically:encoding:)

Writes the contents of the receiver to a file at a given path using a given encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    toFile path: String,
    atomically useAuxiliaryFile: Bool,
    encoding enc: UInt
) throws
```

## Parameters 

`path`  

The file to which to write the receiver. If `path` contains a tilde (`~`) character, you must expand it with expandingTildeInPath before invoking this method.

`useAuxiliaryFile`  

If true, the receiver is written to an auxiliary file, and then the auxiliary file is renamed to `path`. If false, the receiver is written directly to `path`. The true option guarantees that `path`, if it exists at all, won’t be corrupted even if the system should crash during writing.

`enc`  

The encoding to use for the output. For possible values, see NSStringEncoding.

## Discussion

This method overwrites any existing file at `path`.

This method stores the specified encoding with the file in an extended attribute under the name `com.apple.TextEncoding`. The value contains the IANA name for the encoding and the CFStringEncoding value for the encoding, separated by a semicolon. The `CFStringEncoding` value is written as an ASCII string containing an unsigned 32-bit decimal integer and is not terminated by a null character. One or both of these values may be missing. Examples of the value written include the following:

- `MACINTOSH;0`

- `UTF-8;134217984`

- `UTF-8;`

- `;3071`

The methods init(contentsOfFile:usedEncoding:), init(contentsOfURL:usedEncoding:), stringWithContentsOfFile:usedEncoding:error:, and init(contentsOfURL:usedEncoding:) use this information to open the file using the right encoding.

Note

In the future this attribute may be extended compatibly by adding additional information after what’s there now, so any readers should be prepared for an arbitrarily long value for this attribute, with stuff following the `CFStringEncoding` value, separated by a non-digit.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Writing to a File or URL

func write(to: URL, atomically: Bool, encoding: UInt) throws

Writes the contents of the receiver to the URL specified by `url` using the specified encoding.

