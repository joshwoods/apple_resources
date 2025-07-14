

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeySequenceDataIndex
-  charSequenceOffsets 

Instance Property

# charSequenceOffsets

An array of offsets from the beginning of the `UCKeySequenceDataIndex` structure to the Unicode character sequences that follow it. Because a given offset indicates both the beginning of a new character sequence and the end of the sequence that precedes it, the length of each sequence is determined by the difference between the offset to that sequence and the value of the next offset in the array. The array contains one more entry than the number of character sequences; the final entry is the offset to the end of the final character sequence.

Mac Catalyst 13.0+macOS 10.0+

``` source
var charSequenceOffsets: UInt16
```

