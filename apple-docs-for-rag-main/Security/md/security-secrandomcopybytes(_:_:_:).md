

- Security
-  SecRandomCopyBytes(\_:\_:\_:) 

Function

# SecRandomCopyBytes(\_:\_:\_:)

Generates an array of cryptographically secure random bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecRandomCopyBytes(
    _ rnd: SecRandomRef?,
    _ count: Int,
    _ bytes: UnsafeMutableRawPointer
) -> Int32
```

## Parameters 

`rnd`  

The random number generator object to use. Specify kSecRandomDefault to use the default random number generator.

`count`  

The number of random bytes to return in the array pointed to by the `bytes` parameter.

`bytes`  

A pointer to an array that the function fills with cryptographically secure random bytes. Use an array that is large enough to hold at least `count` bytes.

## Return Value

A result code set to errSecSuccess or some other value on failure.

## Discussion

Always test the returned status to make sure that the array has been updated with new, random data before trying to use the values. For example, to create 10 random bytes:

- Swift
- Objective-C

```
var bytes = [Int8](repeating: 0, count: 10)
let status = SecRandomCopyBytes(kSecRandomDefault, bytes.count, &bytes)

if status == errSecSuccess { // Always test the status.
    print(bytes)
    // Prints something different every time you run.
}
```

```
SInt8 bytes[10];
int status = SecRandomCopyBytes(kSecRandomDefault, (sizeof bytes)/(sizeof bytes[0]), &bytes);

if (status == errSecSuccess) { // Always test the status.
    for (int i = 0; i 

