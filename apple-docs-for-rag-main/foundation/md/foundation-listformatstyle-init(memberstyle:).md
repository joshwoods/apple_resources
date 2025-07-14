

- Foundation
- ListFormatStyle
-  init(memberStyle:) 

Initializer

# init(memberStyle:)

Creates an instance using the provided format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(memberStyle: Style)
```

## Parameters 

`memberStyle`  

The FormatStyle applied to elements of the Sequence.

## Discussion

The input type of memberStyle must match the type of an element in the sequence. The output type is a string.

The following example uses a `FloatingPointFormatStyle.Descriptive` member style to spell out a list:

```
[-3.0, 9.0, 11.6].formatted(.list(memberStyle: .descriptive, type: .and))
// minus three, nine, and eleven point six
```

