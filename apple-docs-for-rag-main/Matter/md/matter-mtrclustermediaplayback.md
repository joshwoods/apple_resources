

- Matter
-  MTRClusterMediaPlayback 

Class

# MTRClusterMediaPlayback

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterMediaPlayback
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func fastForward(with: MTRMediaPlaybackClusterFastForwardParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func fastForward(with: MTRMediaPlaybackClusterFastForwardParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func fastForward(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func fastForward(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func next(with: MTRMediaPlaybackClusterNextParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func next(with: MTRMediaPlaybackClusterNextParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func next(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func next(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func pause(with: MTRMediaPlaybackClusterPauseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func pause(with: MTRMediaPlaybackClusterPauseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func pause(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func pause(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func play(with: MTRMediaPlaybackClusterPlayParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func play(with: MTRMediaPlaybackClusterPlayParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func play(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func play(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func previous(with: MTRMediaPlaybackClusterPreviousParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func previous(with: MTRMediaPlaybackClusterPreviousParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func previous(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func previous(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentState(with: MTRReadParams?) -> [String : Any]?

func readAttributeDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributePlaybackSpeed(with: MTRReadParams?) -> [String : Any]?

func readAttributeSampledPosition(with: MTRReadParams?) -> [String : Any]?

func readAttributeSeekRangeEnd(with: MTRReadParams?) -> [String : Any]?

func readAttributeSeekRangeStart(with: MTRReadParams?) -> [String : Any]?

func readAttributeStartTime(with: MTRReadParams?) -> [String : Any]?

func rewind(with: MTRMediaPlaybackClusterRewindParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func rewind(with: MTRMediaPlaybackClusterRewindParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func rewind(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func rewind(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func seek(with: MTRMediaPlaybackClusterSeekParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func seek(with: MTRMediaPlaybackClusterSeekParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func skipBackward(with: MTRMediaPlaybackClusterSkipBackwardParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func skipBackward(with: MTRMediaPlaybackClusterSkipBackwardParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func skipForward(with: MTRMediaPlaybackClusterSkipForwardParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func skipForward(with: MTRMediaPlaybackClusterSkipForwardParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func startOver(with: MTRMediaPlaybackClusterStartOverParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func startOver(with: MTRMediaPlaybackClusterStartOverParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func startOver(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func startOver(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func stop(with: MTRMediaPlaybackClusterStopParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func stop(with: MTRMediaPlaybackClusterStopPlaybackParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func stop(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func stop(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func activateAudioTrack(with: MTRMediaPlaybackClusterActivateAudioTrackParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func activateTextTrack(with: MTRMediaPlaybackClusterActivateTextTrackParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func deactivateTextTrack(with: MTRMediaPlaybackClusterDeactivateTextTrackParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func deactivateTextTrack(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

## Relationships

### Inherits From

- MTRGenericCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

