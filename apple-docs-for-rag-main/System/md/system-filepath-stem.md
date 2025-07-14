

- System
- FilePath
-  stem 

Instance Property

# stem

The non-extension portion of the file or directory last component.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var stem: String? { get }
```

## Discussion

Returns `nil` if `lastComponent` is `nil`

- `/tmp/foo.txt => foo`

- `/Applications/Foo.app/ => Foo`

- `/Applications/Foo.app/bar.txt => bar`

- `/tmp/.hidden => .hidden`

- `/tmp/.. => ..`

- `/ => nil`

