

- SensorKit
- SRKeyboardMetrics
-  totalPauses 

Instance Property

# totalPauses

The total number of pauses during the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var totalPauses: Int { get }
```

## Discussion

The framework records a pause when the user stops entering text for more than 5 seconds.

## See Also

### Quantifying Key Use

var totalWords: Int

The total number of typed words for the keyboard.

var totalAlteredWords: Int

The total number of altered words for the keyboard.

var totalTaps: Int

The total number of taps for the keyboard.

var totalDrags: Int

The total number of drags for the keyboard.

var totalDeletes: Int

The total number of deletions for the keyboard.

var totalEmojis: Int

The total number of emojis for the keyboard.

var totalPaths: Int

The total number of completed paths for the keyboard.

var totalPathTime: TimeInterval

The total time to complete paths for the keyboard.

var totalPathLength: Measurement&lt;UnitLength>

The total length of completed paths for the keyboard.

var totalAutoCorrections: Int

The total number of autocorrections for the keyboard.

var totalSpaceCorrections: Int

The total number of space corrections for the keyboard.

var totalRetroCorrections: Int

The total number of retro corrections for the keyboard.

var totalTranspositionCorrections: Int

The total number of transposition corrections for the keyboard.

var totalInsertKeyCorrections: Int

The total number of Insert key corrections for the keyboard.

var totalSkipTouchCorrections: Int

The total number of skip touch corrections for the keyboard.

