<!--
Downloaded via https://llm.codes by @steipete on June 19, 2025 at 07:44 PM
Source URL: https://developer.apple.com/documentation/http-live-streaming
Total pages processed: 47
URLs filtered: Yes
Content de-duplicated: Yes
Availability strings filtered: Yes
Code blocks only: No
-->

# https://developer.apple.com/documentation/http-live-streaming

# HTTP Live Streaming

Send audio and video to iOS, tvOS, and macOS devices.

## Overview

HTTP Live Streaming (HLS) sends audio and video over HTTP from an ordinary web server for playback on iOS-based devices—including iPhone, iPad, iPod touch, and Apple TV—and on desktop computers (macOS). Using the same protocol that powers the web, HLS deploys content using ordinary web servers and content delivery networks. HLS is designed for reliability and dynamically adapts to network conditions by optimizing playback for the available speed of wired and wireless connections.

HLS supports the following:

- Live broadcasts and prerecorded content (video on demand, or VOD)

- Multiple alternate streams at different bit rates

- Intelligent switching of streams in response to network bandwidth changes

- Media encryption and user authentication

### Encode and deliver streaming media

The following figure shows the three components of an HTTP Live Stream: the server component, the distribution component, and the client software.

In a typical configuration, a hardware encoder takes audio-video input, encodes it as HEVC video and AC-3 audio, and outputs a fragmented MPEG-4 file or an MPEG-2 transport stream. A software stream segmenter then breaks the stream into a series of short media files, which are placed on a web server. The segmenter also creates and maintains an index file containing a list of the media files. The URL of the index file is published on the web server. Client software reads the index, then requests the listed media files in order and displays them without any pauses or gaps between segments.

### Prepare media with the server component

The server component is responsible for taking input streams of media and encoding them digitally. It encapsulates them in a format suitable for delivery and prepares the encapsulated media for distribution.

For live events, the server requires a media encoder, which can be off-the-shelf hardware, and a way to break the encoded media into segments and save them as files, which can either be software such as the media stream segmenter provided by Apple or part of an integrated third-party solution.

### Deliver files with the distribution component

The distribution system is a web server or a web-caching system that delivers the media files and index files to the client over HTTP. No custom server modules are required to deliver the content, and typically very little configuration is needed on the web server. To actually deploy HTTP Live Streaming, you need to create either an HTML page for browsers or a client app to act as a receiver. You also need the use of a web server and a way to encode live streams as fragmented MPEG-4 media files containing HEVC or H.264 video, and AAC or AC-3 audio.

### Access media through client software

Client software is responsible for determining the appropriate media to request, downloading those resources, and then reassembling them so that the media can be presented to the user in a continuous stream. For the rules governing the interaction between an HLS player and its server, see HTTP Live Streaming 2nd Edition.

Apple provides several frameworks that support HTTP Live Streaming, including AVKit, AVFoundation, and WebKit. Support has been available since iOS 3.0 and Safari 4.0, so there’s no need to develop your own client software.

However, if you do develop your own client software, begin by fetching the index file using a URL that identifies the stream. The index file, in turn, specifies the location of the available media files, decryption keys, and any alternate streams available. For the selected stream, download each available media file in sequence. Each file contains a consecutive segment of the stream. Once it has a sufficient amount of data downloaded, present the reassembled stream to the user.

Continue this process until your client encounters the `EXT-X-ENDLIST` tag in the index file. If no `EXT-X-ENDLIST` tag is present, the index file is part of an ongoing broadcast. During ongoing broadcasts, load a new version of the index file periodically. Look for new media files and encryption keys in the updated index and add these URLs to the playback queue.

## Topics

### Essentials

Deploying a Basic HTTP Live Streaming (HLS) Stream

Create a basic webpage to deliver HLS.

Preparing Audio for HTTP Live Streaming

Encode your media properly to ensure synchronized audio and video playback.

### Stream creation

Learn to create a stream for ingestion by apps enabled with HTTP Live Streaming. Ensure correct playlist formatting and adherence to guidelines.

View and compare playlists for different HLS applications.

About the EXT-X-VERSION tag

Find the protocol version that corresponds with the HLS features your app supports.

### Tool usage and validation

Use the provided tools to segment your stream, create multivariant playlists, and verify the output of your own tools.

Using Apple’s HTTP Live Streaming (HLS) Tools

Segment your video stream and create media playlists for successful transmission with Apple’s provided tools.

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/deploying-a-basic-http-live-streaming-hls-stream

- HTTP Live Streaming
- Deploying a Basic HTTP Live Streaming (HLS) Stream

Article

# Deploying a Basic HTTP Live Streaming (HLS) Stream

Create a basic webpage to deliver HLS.

## Overview

An HLS stream may either be live or on-demand (VOD). The requirements for deploying an HLS stream are:

- Either an HTML page for browsers or a client app to act as a receiver

- A web server or CDN to act as a host

- A way to encode your source material or live streams as fragmented MPEG-4 media files containing HEVC or H.264 video and AAC or AC-3 audio. Although you can use MP3 audio files or MPEG-2 transport streams for H.264 video, these formats aren’t recommended.

### Create an HTML page

### Configure a web server

HLS streams can be served from an ordinary web server. Configure your web server and associate the MIME types of the files being served with their file extensions. The following table shows the MIME types for HLS.

| File Extension | MIME Type |
| --- | --- |
| `.m3u8` | `vnd.apple.mpegURL` |
| `.ts` | `video/MP2T` |
| `.mp4` | `video/mp4` |

If your web server is constrained with respect to MIME types, you can serve files ending in `.m3u` with MIME type `audio/mpegURL` for compatibility.

Index files are often long and are frequently redownloaded, but because they’re text files, they can be compressed very efficiently. Reduce server overhead by enabling real-time `gzip` compression of `M3U8` index files. The HTTP Live Streaming client automatically unzips compressed index files.

You might need to shorten time-to-live (TTL) values for M3U8 files to achieve proper caching behavior for downstream web caches. M3U8 files are frequently overwritten during live broadcasts, and the latest version should be downloaded for each request. Check with your content delivery service provider for specific recommendations. For VOD, the index file is static and is downloaded only once, so caching isn’t a factor.

### Validate your streams

The `mediastreamvalidator` tool is a command-line utility for validating HLS streams and servers. See Using Apple’s HTTP Live Streaming (HLS) Tools for details on obtaining the tool.

The media stream validator simulates an HLS session and verifies that the index file and media segments conform to the HLS specification. It performs several checks to ensure reliable streaming. If any errors or problems are found, a detailed diagnostic report is displayed. Always run the validator prior to serving a new stream or alternate stream set.

See FairPlay Streaming for details on validating with secure protocols.

### Serve key files securely over HTTPS

Protect your media by encrypting it. The file segmenter and stream segmenter tools both have encryption options, and you can configure them to change the encryption key periodically. Who you share the keys with is up to you.

Key files require an initialization vector to decode encrypted media. The initialization vectors can be changed periodically, just as the keys can. The current recommendation for encrypting media while minimizing overhead is to change the key every 3 to 4 hours and change the initialization vector after every 50 Mb of data.

Even with restricted access to keys, it’s possible for an eavesdropper to obtain copies of the key files if they’re sent over HTTP. One solution to this problem is to send the keys securely over HTTPS. Before attempting to serve key files over HTTPS, test serving the keys from an internal web server over HTTP. This allows you to debug your setup before adding HTTPS to the mix. Once you have a known working system, you can make the switch to HTTPS.

The requirements for using HTTPS to serve keys for HLS are:

- Verify that you have an SSL certificate signed by a trusted authority on your HTTPS server. If not, you can still test your setup by creating a self-signed SSL Certificate Authority and a leaf certificate for your server. Attach the certificate for the certificate authority to an email, send it to a device you want to use as an HLS client, and tap the attachment in Mail to make the device trust the server.

- Ensure that the authentication domain for the key files is the same as the authentication domain for the first playlist file. The simplest way to accomplish this is to serve the Multivariant Playlist file from the HTTPS server. The playlist file is downloaded once, so this shouldn’t cause an excessive burden. Other playlist files can be served using HTTP.

- Either initiate your own dialog for the user to authenticate, or store the credentials on the client device. HLS doesn’t provide user dialogs for authentication. If you’re writing your own client app, you can store cookie-based or HTTP credentials and supply them in the `connection(_:didReceive:)` callback. The credentials you supply are cached and reused by the media player.

A sample-level encryption format is documented in MPEG-2 Stream Encryption Format for HTTP Live Streaming. For the strongest level of content protection, an alternative to serving keys directly over HTTPS is to use FairPlay Streaming. See HTTP Live Streaming (HLS) authoring specification for Apple devices for more information.

## See Also

### Essentials

Preparing Audio for HTTP Live Streaming

Encode your media properly to ensure synchronized audio and video playback.

---

# https://developer.apple.com/documentation/http-live-streaming/preparing-audio-for-http-live-streaming

- HTTP Live Streaming
- Preparing Audio for HTTP Live Streaming

Article

# Preparing Audio for HTTP Live Streaming

Encode your media properly to ensure synchronized audio and video playback.

## Overview

Producing media for HTTP Live Streaming (HLS) requires special considerations if you’re encoding audio using the Advanced Audio Coding (AAC) family of formats.

AAC audio processing requires a small amount of leading “throw-away” audio to prime the encoder and initialize internal tables. This small amount of audio results from _encoder delay_ which happens during encoding to produce properly formed, encoded audio packets, and its duration is commonly referred to as the _priming duration_. This audio needs to occur before the first frame of video; otherwise, there will be no audio for the first few frames of video.

The audio sample rates are normally 44.1 kHz or 48 kHz. For more information, see the HTTP Live Streaming Specification and the HTTP Live Streaming (HLS) authoring specification for Apple devices.

### Encode MPEG-2 transport stream segments

MPEG-2 transport streams create an arbitrary timestamp when encoding media, using an 33-bit clock that rolls over every 26 hours. For example, if your video starts at the two-hour mark, your audio starts at two hours plus the time for the leading audio. Therefore, a segment of audio that’s paired with a segment of video starting at the two-hour mark needs audio that starts at the two-hour mark minus the priming duration. This additional segment ensures the first frame of video plays synchronously with the audio.

### Encode fragmented MPEG-4 segments

The MPEG-4 file format (ISO BMFF) carries the presumption that all track timelines begin with time zero, regardless of whether the timeline is divided into fragments. However, you can set the initial decode time of any fragment to an arbitrary value by means of the Track Fragment Base Media Decode Time Box ( `tfdt`). Use this box to permit the alignment of the audio timeline with the video timeline that places the priming audio prior to the first video frame.

Alternatively, starting with iOS 13.1 it’s possible to utilize an Edit List Box ( `elst`) within the Track Box ( `trak`) in order to place the duration of the priming audio prior to time 0. This permits a natural alignment of other tracks with audio at time 0. The edit list needs to have a single entry in which the value of `media_start` is equivalent to the audio priming duration and the value of `segment_duration` is 0. This is the recommended approach for time alignment for the Common Media Application Format (CMAF).

### Handle play position changes within content

Changing the play position to a specific point in time within content is known as _seeking_, and is another consideration for encoding audio. HTTP Live Streaming (HLS) has individual segments that are individually downloadable; each contains media data for 4 to 6 seconds of the overall media timeline. When seeking into a point in the video, skip over the intervening segments between the current and target play position and load the appropriate segment.

## See Also

### Essentials

Deploying a Basic HTTP Live Streaming (HLS) Stream

Create a basic webpage to deliver HLS.

---

# https://developer.apple.com/documentation/http-live-streaming/example-playlists-for-http-live-streaming

Collection

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming

# Example playlists for HTTP Live Streaming

View and compare playlists for different HLS applications.

## Overview

HTTP Live Streaming sends audio and video as a series of small files, typically of about 6 seconds duration, called _media segment files_. An index file, or playlist, provides an ordered list of the URLs of the media segment files. Index files for HTTP Live Streaming are saved as M3U8 playlists, an extension of the M3U format used for MP3 playlists. The URL of the index file is accessed by clients, which then request the indexed files in sequence.

You can use the Apple HTTP Live Streaming tools to generate playlists. These tools are frequently updated and you can get them from Downloads for Apple Developers if you’re a member of the Apple Developer Program. See Using Apple’s HTTP Live Streaming (HLS) Tools for more information about the individual tools.

## Topics

### Basic playlists

Video on Demand playlist construction

Understand the basic composition for a Video on Demand playlist.

Live Playlist (sliding window) construction

Understand the basic composition for a live session playlist.

Event playlist construction

Learn about the basic composition of an event session playlist.

Creating a Multivariant Playlist

Offer multiple playlist files to provide different encodings of the same content.

### Modified playlists

Incorporating Ads into a Playlist

Add branding or ads to a playlist.

Adding alternate media to a playlist

Specify Rendition Playlists that can override the main presentation.

## See Also

### Stream creation

About the EXT-X-VERSION tag

Find the protocol version that corresponds with the HLS features your app supports.

---

# https://developer.apple.com/documentation/http-live-streaming/about-the-ext-x-version-tag

- HTTP Live Streaming
- About the EXT-X-VERSION tag

Article

# About the EXT-X-VERSION tag

Find the protocol version that corresponds with the HLS features your app supports.

## Overview

The `EXT-X-VERSION` tag indicates the compatibility version of the Playlist file. This file, its associated media, and its server must comply with all provisions of the IETF Internet-Draft of HTTP Live Streaming 2nd Edition (or earlier specifications) describing the protocol version indicated by the tag value. A Playlist file that doesn’t contain an `EXT-X-VERSION` tag must comply with version 1 of this protocol. Support for M3U8 Playlists was introduced with iOS 3.0, Mac OS X 10.6, and Safari 4.

### High-level features

| EXT-X-VERSION | Features and usage notes |
| --- | --- |
| 2 | IV attribute of the `EXT-X-KEY` tag |
| 3 | Floating-point `EXTINF` duration values |
| 4 | `EXT-X-BYTERANGE`, `EXT-X-I-FRAME-STREAM-INF`, ` EXT-X-I-FRAMES-ONLY`, `EXT-X-MEDIA`, the `AUDIO` and `VIDEO` attributes of the `EXT-X-STREAM-INF` tag |
| 5 | `KEYFORMAT` and `KEYFORMATVERSIONS` attributes of the `EXT-X-KEY` tag. The `EXT-X-MAP` tag. `SUBTITLES` media type. `SAMPLE-AES` encryption method `EXT-X-KEY` |
| 6 | `CLOSED-CAPTIONS` media type. Allow ` EXT-X-MAP` for subtitle playlists |
| 7 | `EXT-X-SESSION-DATA`, `EXT-X-SESSION-KEY`, `EXT-X-DATERANGE`, `SERVICE` _**n**_ values of `INSTREAM-ID`, `AVERAGE-BANDWIDTH`, `FRAME-RATE`, `CHANNELS`, and `HDCP-LEVEL` attributes. |
| 8 | `EXT-X-GAP`, `EXT-X-DEFINE`, Variable Substitution, `VIDEO-RANGE` attribute. |
| 9 | `EXT-X-SKIP` |
| 10 | `EXT-X-SERVER-CONTROL`, `EXT-X-PART-INF`, `EXT-X-PRELOAD-HINT`, `EXT-X-RENDITION-REPORT`, the `CUE` attribute of `EXT-X-DATERANGE`, the `STABLE-RENDITION-ID` of `EXT-X-MEDIA`, the `SUPPLEMENTAL-CODECS` attribute of `EXT-X-STREAM-INF`, and the `SCORE` and `STABLE-VARIANT-ID` attributes of `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF` tags |
| 11 | `QUERYPARAM` attribute of `EXT-X-DEFINE` |
| 12 | Attributes starting with ‘ `REQ-`’ |

### Backward compatibility

The following features aren’t backward compatible. Older clients may fail to play the content if you use these features but don’t specify the protocol version where they were introduced:

- You must use at least protocol version 2 if you have `IV` in `EXT-X-KEY`.

- You must use at least protocol version 3 if you have floating point `EXTINF` duration values.

- You must use at least protocol version 4 if you have `EXT-X-BYTERANG` E or `EXT-X-IFRAME-ONLY`.

- You must use at least protocol version 5 if you specify the `SAMPLE-AES` encryption method in `EXT-X-KEY`, or if you have `KEYFORMAT` and `KEYFORMATVERSIONS` attributes in `EXT-X-KEY`, or if you have `EXT-X-MAP`.

- You must use at least protocol version 6 if you have `EXT-X-MAP` in a Media Playlist that does not contain `EXT-X-I-FRAMES-ONLY`.

- You must use at least protocol version 7 if you specify `SERVICE` _**n**_ values for the `INSTREAM-ID` attribute of `EXT-X-MEDIA`.

- You must use at least protocol version 8 if you use variable substitution.

- You must use at least protocol version 9 if you have `EXT-X-SKIP`.

- You must use at least protocol version 10 if you have `EXT-X-SKIP` that replaces `EXT-X-DATERANGE` tags in a Playlist Delta Update.

- You must use at least protocol version 11 if you have `QUERYPARAM` attribute in `EXT-X-DEFINE`.

- You must use at least protocol version 12 if you have attributes that start with “ `REQ-`”.

### Specifications

The following tables list the versions of specifications where specific features are described, along with the corresponding iOS release that supports those features.

### draft-pantos-http-live-streaming and RFC 8216

| Revision | iOS Version | Notes |
| --- | --- | --- |
| 00, 01 | 3.0 | **Protocol version 1**. Initial version. |
| 02 | 3.1 | Added `EXT-X-DISCONTINUITY`. Changed Content-Type. Added redundant streams. |
| 03, 04 | 3.2 | **Protocol version 2**. Added `EXT-X-VERSION`. Added IV attribute to `EXT-X-KEY`; `RESOLUTION` attribute to `EXT-X-STREAM-INF`. Corrected `CODECS` attribute values. |
| — | 4.0 | Added timed metadata APIs, custom protocols for keys. |
| 05 | 4.2 | **Protocol version 3**. Added `EXTINF` floating point durations. Support for CEA-608 Closed captions. |
| — | 4.3 | Added `AccessLog` & `ErrorLog` objects to APIs. |
| 06 | 4.3.2 | Added `EXT-X-PLAYLIST-TYPE`. |
| 07, 08 | 5.0 | **Protocol version 4**. Added `EXT-X-I-FRAMES-ONLY`; `EXT-X-I-FRAME-STREAM-INF`; `EXT-X-MEDIA`; `EXT-X-BYTERANGE`. Added `AUDIO` and `VIDEO` attributes to `EXT-X-STREAM-INF`. |
| 09, 10, 11 | 6.0 | **Protocol version 5**. Added `EXT-X-MAP`. Added `KEYFORMAT` and `KEYFORMATVERSIONS` attributes to `EXT-X-KEY`; `SUBTITLES` attribute to `EXT-X-STREAM-INF`; `FORCED` and `CHARACTERISTICS` attributes to `EXT-X-MEDIA`. Added `SUBTITLES` value to `TYPE` attribute of ` EXT-X-MEDIA`; `SAMPLE-AES` value to `METHOD` attribute of `EXT-X-KEY`. Added `X-TIMESTAMP-MAP` to WebVTT. Added AC-3 support. |
| 12 | 7.0 | **Protocol version 6**. Added `EXT-X-DISCONTINUITY-SEQUENCE`; `EXT-X-START`. Added `ASSOC-LANGUAGE` and `INSTREAM-ID` attributes to `EXT-X-MEDIA`; `CLOSED-CAPTIONS` attribute to `EXT-X-STREAM-INF`. Removed `PROGRAM-ID` attribute of `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Added `CLOSED-CAPTIONS` value to `TYPE` attribute of `EXT-X-MEDIA`. Allow `EXT-X-MAP` to be used in subtitle playlists. |
| 13 | 7.1 | Added `EXT-X-INDEPENDENT-SEGMENTS`. |
| 14, 15, 16 | 8.0 | P **rotocol version 7**. Major re-write of spec. Added `EXT-X-SESSION-DATA`. Removed `EXT-X-ALLOW-CACHE`. Added `AVERAGE-BANDWIDTH` attribute to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Added `SERVICE` _**n**_ values to `INSTREAM-ID` attribute of `EXT-X-MEDIA`. Added support for Enhanced AC-3. Support for CEA-708 Closed captions. |
| 17, 18 | 9.0 | Added `EXT-X-SESSION-KEY`. Added `FRAME-RATE` to `EXT-X-STREAM-INF` and `EXT-X-IFRAME-STREAM-INF`. New peak bit-rate calculation. |
| 19 | 9.3 | Added `EXT-X-DATERANGE`. |
| 20 | 10.0 | Added `CHANNELS` attribute to `EXT-X-MEDIA`; `HDCP-LEVEL` attribute to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Added fMP4 support. |
| 21, 22, 23 | 10.3.1 | Clarified `AUTOSELECT=YES` uniqueness. Added mention of CMAF. |
| RFC8216 | 10.3.1 | Wording changes and clarifications. |

### draft-pantos-hls-rfc8216bis

| Revision | iOS Version | Notes |
| --- | --- | --- |
| 00 | 11.0 | **Protocol version 8**. Added `EXT-X-GAP`; `EXT-X-DEFINE` and Variable Substitution. Added `VIDEO-RANGE` attribute to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Added `TYPE-1` value to `HDCP-LEVEL` attribute. Support for `IMSC1` subtitles. |
| 01 | - | Clarified the `X-TIMESTAMP-MAP` for non-MPEG-2 content. Added semantic change for `EXT-X-TARGETDURATION` tag. Updated the JSON RFC format requirement. |
| 02 | 12.0 | Added second `CHANNELS` parameter. Added unrecognized `CHANNELS` parameters guidance. |
| 03 | - | Added `EXT-X-BITRATE` tag. Minor clarification about the use of Movie Extends Box in Fragmented MPEG-4 files. |
| 04 | - | Add note about PES timestamp wraps. |
| 05 | 13.0 | Revise definition of peak segment bit rate. Add `ALLOWED-CPC` attribute to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Allow Media Metadata tags to be removed from playlists. |
| 06 | - | Rearranged Playlist Tags subsections. Minor rewording. |
| 07 | 13.5 | **Protocol version 10**. Support for Low-Latency HLS, including Partial Segments, Delivery Directives, Playlist Delta Updates, and the Low-Latency Server Configuration Profile. Adds tags: `EXT-X-PART-INF`, `EXT-X-SERVER-CONTROL`, `EXT-X-PART`, `EXT-X-SKIP`, `EXT-X-PRELOAD-HINT`, and `EXT-X-RENDITION-REPORT`. Adds `HLG` enum value to `VIDEO-RANGE` attribute. Reserves query parameters that begin with “ `_HLS_`”. |
| 08 | 14.0 | Add `SCORE` and `STABLE-VARIANT-ID` attributes to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Add `STABLE-RENDITION-ID` attribute to `EXT-X-MEDIA`. `CHARACTERISTICS` values are Media Characteristic Tags, not Uniform Type Identifiers. A few minor clarifications. |
| 09 | - | Minor clarifications. Preload hint request should use 2^53-1 for unknown byte range length. |
| 10 | 15.0 | Rename to “Multivariant Playlist”. Add Content Steering ( `EXT-X-CONTENT-STEERING` tag, `PATHWAY-ID` attribute, and fetching Steering Manifests). Add Interstitials (specialized `EXT-X-DATERANGE` tags, asset list interstitial JSON files, and the enumerated-string-list type). Minor clarifications. |
| 11 | 15.5 | Update Content Steering to add Pathway Cloning. Add `CUE` attribute to `EXT-X-DATERANGE`. Add `SUPPLEMENTAL-CODECS` attribute to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Minor clarifications. |
| 12 | 16.0 | Document `_HLS_start_offset`. Modify rules for Partial Segments near `GAP` s. Relax `EXT-X-DATERANGE` rules for Renditions. Minor clarifications. |
| 13 | 16.5 | **Protocol version 12**. Add `QUERYPARAM` attibute to `EXT-X_DEFINE`. Add `FORMAT` attribute to `EXT-X-SESSION-DATA`. Add special behavior for attributes with a prefix of “ `REQ-`”. Some clarifications. |
| 14 | 17.0 | Added `BIT-DEPTH` and `SAMPLE-RATE` attributes to `EXT-X-MEDIA`. Extended `CHANNELS` attribute of `EXT-X-MEDIA` to allow a third parameter. Added `REQ-VIDEO-LAYOUT` attribute to `EXT-X-STREAM-INF` and `EXT-X-I-FRAME-STREAM-INF`. Added mention of the extensible priority scheme. Added appendix on “Displaying Rendition Names”. Minor clarifications. |
| 15 | 17.5 | Added mention of `SAMPLE-AES-CTR` method of `EXT-X-KEY`. Some clarifications. |

## See Also

### Stream creation

View and compare playlists for different HLS applications.

---

# https://developer.apple.com/documentation/http-live-streaming/using-apple-s-http-live-streaming-hls-tools

- HTTP Live Streaming
- Using Apple’s HTTP Live Streaming (HLS) Tools

Article

# Using Apple’s HTTP Live Streaming (HLS) Tools

Segment your video stream and create media playlists for successful transmission with Apple’s provided tools.

## Overview

Apple provides HLS Tools to help you set up an HLS service. HLS Tools update frequently; you can download the current versions from the Apple Developer Downloads website. To access them, sign in with the Apple ID associated with your developer account.

### Download the tools

The download package contains the following tools:

- **Media File Segmenter** ( `mediafilesegmenter`) divides a transport stream input or file — such as an MOV, MP4, M4V, M4A, or MP3 — into media segments, creates a media playlist, and can also perform segment encryption. You can deploy the media playlist and media segments using almost any web server infrastructure for streaming to iOS, macOS, and tvOS. The Media File Segmenter only produces Video-on-Demand (VOD) streams.

- **Media Subtitle Segmenter** ( `mediasubtitlesegmenter`) converts subtitle tracks from a QuickTime file with tx3g-formatted subtitle tracks or SRT files into WebVTT, then segments them for deployment using HLS. It also segments WebVTT files.

- **Media Stream Segmenter** ( `mediastreamsegmenter`) receives an MPEG-2 transport stream over a UDP network connection or an input stream on a local port and packages it for HLS. It writes a single live Media Playlist with its corresponding Media Segments (including Partial Segments in Low-Latency mode) and can also perform segment encryption. The Media Stream Segmenter writes its output to the local file system or a WebDAV endpoint. You can deploy the live Media Playlist and Segments using almost any web server infrastructure for streaming to iOS, macOS, and tvOS. The Media Stream Segmenter produces either live or VOD streams.

- **Variant Playlist Creator** ( `variantplaylistcreator`) works with Media File Segmenter to create a multivariant playlist from multiple VOD streams.

- **Media Stream Validator** ( `mediastreamvalidator`) simulates an HLS session and verifies that the media playlist and media segments conform to the HLS specification. This tool can validate local files and HTTP URLs.

- **HLS Report** ( `hlsreport`) uses the JSON file generated by Media Stream Validator to create a report for the validated stream.

- **ID3 Tag Generator** ( `id3taggenerator`) creates ID3 tags as metadata for the Media File Segmenter or sends them over the network to the Media Stream Segmenter.

- **TS Recompressor** ( `tsrecompressor`) uses a file or standard input to produce and encode up to four continuous audio and video streams at different bit rates. It multicasts them as MPEG-2 Transport Streams to local UDP ports. The tool can produce content programmatically, or capture video from the system camera and microphone. In programmatic mode, it creates a test pattern stream that features burnt-in timecode video and linear timecode audio. Both presentations use real-time Society of Motion Picture and Television Engineers (SMPTE) timecodes derived from the system clock.

- **Low-Latency HLS Golang script** ( `ll-hls-origin-example.go`) implements the HLS Origin API for a Low-Latency HLS media playlist.

- **Low-Latency HLS PHP script** ( `lowLatencyHLS.php`) implements the HLS Origin API for a Low-Latency HLS media playlist. It can be used as an alternative to the Low-Latency HLS Golang script.

When creating your own tools or using a third-party tool, ensure that the tool output conforms to Apple’s standards.

---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices

Collection

- HTTP Live Streaming
- HTTP Live Streaming (HLS) authoring specification for Apple devices

# HTTP Live Streaming (HLS) authoring specification for Apple devices

Learn the requirements for live and on-demand audio and video content delivery using HLS.

## Overview

For a deeper discussion of the features available in HLS, refer to Apple’s streaming resource page, which contains pointers to the overview document, the HLS specification, technical notes, tools, presentations, and examples.

### About HLS authoring

The HLS specification is a published RFC ( RFC 8216). However, HLS continues to evolve, so there’s an updated draft specification — draft-pantos-hls-rfc8216bis (HLS2).

Please see Documentation, which may contain a reference to a preliminary version of the draft specification.

This document always uses the most up-to-date version, which is, either the preliminary version or the draft specification (whichever has a higher version number).

The key words “MUST,” “MUST NOT,” “REQUIRED,” “SHALL,” “SHALL NOT,” “SHOULD,” “SHOULD NOT,” “RECOMMENDED,” “MAY,” and “OPTIONAL” in this document are to be interpreted as described in RFC 2119.

Find additional information for HLS specifications at HTTP Live Streaming (HLS) Authoring Specification for Apple devices appendixes.

### About spatial video

Spatial video is intended to produce a richer experience for the user. Spatial video MUST use the REQ-VIDEO-LAYOUT attribute to specify desired channel and projection specifiers. Please see HLS specification \[https://developer.apple.com/streaming/HLS-draft-pantos.pdf\] for valid channel and projection specifiers.

Spatial video media is split into following categories.

Stereo Video

Similar to Stereo audio, which indicates different audio for the left and the right ear, visual media can be stereoscopic in which a separate view is available for the left eye and another view is available to be presented simultaneously to the right eye.

Projection Video

Rectilinear projection is default for the video media which indicates there is no further processing necessary to present the video. Content creators can opt for non rectilinear projections to preserve the artistic intent. Please refer to HLS specification \[https://developer.apple.com/streaming/HLS-draft-pantos.pdf\] for possible non-rectilinear projections. This content is categorized under Apple Projected Media Profile (APMP) and can be monoscopic or stereo.

Immersive Video

This video is projected from a hemisphere (typically a special lens) and often requires a special metadata file in order render correctly.

This video relies on a special projection type, known as ‘PROJ-AIV’ which is defined outside the core HLS specification. For details, see \[QuickTime and ISO Base Media File Formats and Spatial and Immersive Media\] (https://developer.apple.com/av-foundation/Stereo-Video-ISOBMFF-Extensions.pdf)

### About multi-format audio codecs

Multi-format audio codecs support combinations of channels, audio objects, and ambisonics as opposed to multi-channel codecs that just support channels. Examples of such a multi-format codec are:

- Apple Positional Audio Codec \[APAC\] (https://developer.apple.com/av-foundation/Apple-Positional-Audio-Codec.pdf)

- Dolby Digital Plus JOC

### General authoring requirements

A stream that matches these requirements should be compatible with iOS, tvOS, macOS or visionOS. Rules with a leading asterisk (\*) are modified by one or more of the Amended Requirements listed below.

Support for a specific video Profile and Level doesn’t imply that any particular device supports the maximum bit rate for that Level.

#### Video

1\. **Video encoding requirements**

1.1. All video MUST be encoded using H.264/AVC, HEVC/H.265, Dolby Vision, or AV1.

1.2. The container format for H.264 video MUST be fragmented MP4 (fMP4) files or MPEG transport streams.

1.3.

1.3a. \* For maximum compatibility, some H.264 variants SHOULD be less than or equal to High Profile, Level 4.1.

1.3b. \* Profile and Level for H.264 MUST be less than or equal to High Profile, Level 5.2.

1.4. For H.264, you SHOULD use High Profile in preference to Main or Baseline Profile.

1.5. The container format for HEVC video MUST be fMP4.

1.6.

1.6a. \* For maximum compatibility, some HEVC variants SHOULD be less than or equal to Main 10 Profile, Level 4.0, Main Tier.

1.6b. \* Profile, Level, and Tier for HEVC MUST be less than or equal to Main 10 Profile, Level 5.1, High Tier.

1.7. High Dynamic Range (HDR) HEVC video MUST be HDR10, HLG, or Dolby Vision.

1.8. For HDR10 video, the `SEI NAL` units (that is, static metadata) SHOULD be in the HEVC Configuration Box ( `'hvcC'`) and not in the individual sample data.

1.9. \* Profile and Level for Dolby Vision MUST be Profile 5 (single layer 10-bit HEVC) and less than or equal to Level 7.

1.10. You SHOULD use video formats in which the parameter sets are stored in the sample descriptions, rather than the samples. (That is, use `'avc1'`, `'hvc1'`, or `'dvh1'` rather than `'avc3'`, `'hev1'`, or `'dvhe'`.)

1.11. For backward compatibility, content SHOULD NOT use a higher level than required by the content resolution and frame rate.

1.12. \* For backward compatibility, some video content SHOULD be encoded with H.264.

1.13. Key frames (IDRs) SHOULD be present every two seconds.

1.14. All interlaced source content MUST be deinterlaced.

1.15. You SHOULD deinterlace 30i content to 60p instead of 30p.

1.16. Live (linear) video from NTSC or ATSC source SHOULD be 60 or 59.94 fps.

1.17. Live (linear) video from PAL source SHOULD be 50 fps.

1.18. Video on Demand (VOD) content SHOULD use a natural frame rate for the content. Frame rates 23.976, 24, 25, 29.97, 30, 50, 59.94, and 60 fps are supported.

1.19. Frame rates above 60 fps SHALL NOT be used.

1.20. \* For HDR content, frame rates less than or equal to 30 fps SHOULD be provided.

1.21. Streams SHOULD use a single color space — one of either Rec. 601, Rec. 709, DCI-P3, or Rec. 2020.

1.22. For VOD, the color space SHOULD be the original color space of the material.

1.23. \* If multiple video streams are provided (H.264, HEVC, HDR), each stream SHOULD provide all anticipated bandwidths. Clients SHOULD NOT be required to switch codecs.

1.24. \* For backward compatibility, SDR streams MUST be provided. (See also item 6.16.)

1.25. \* There are many possible choices of bit rates for variants. The following tables provide one possible set of bit rate variants. (See On bit rates for variants for additional considerations.)

| 16:9 aspect ratio | H.264/AVC | Frame rate |
| --- | --- | --- |
| 416 x 234 | 145 | ≤ 30 fps |
| 640 x 360 | 365 | ≤ 30 fps |
| 768 x 432 | 730 | ≤ 30 fps |
| 768 x 432 | 1100 | ≤ 30 fps |
| 960 x 540 | 2000 | Same as source |
| 1280 x 720 | 3000 | Same as source |
| 1280 x 720 | 4500 | Same as source |
| 1920 x 1080 | 6000 | Same as source |
| 1920 x 1080 | 7800 | Same as source |

| 16:9 aspect ratio | HEVC/H.265 30 fps | HDR (HEVC) 30 fps | Frame rate |
| --- | --- | --- | --- |
| 640 x 360 | 145 | 160 | ≤ 30 fps |
| 768 x 432 | 300 | 360 | ≤ 30 fps |
| 960 x 540 | 600 | 730 | ≤ 30 fps |
| 960 x 540 | 900 | 1090 | ≤ 30 fps |
| 960 x 540 | 1600 | 1930 | Same as source |
| 1280 x 720 | 2400 | 2900 | Same as source |
| 1280 x 720 | 3400 | 4080 | Same as source |
| 1920 x 1080 | 4500 | 5400 | Same as source |
| 1920 x 1080 | 5800 | 7000 | Same as source |
| 2560 x 1440 | 8100 | 9700 | Same as source |
| 3840 x 2160 | 11600 | 13900 | Same as source |
| 3840 x 2160 | 16800 | 20000 | Same as source |

Following tables provide a possible bit rate recommendations for APMP videos.

#### APMP monoscopic videos:

| Tier | Resolution | Bit rate | Projection specifier | fps |
| --- | --- | --- | --- | --- |
| 1 | 8k x 4k | 80 Mbps | PROJ-EQUI | 60 |
| 2 | 8k x 4k | 60 Mbps | PROJ-EQUI | 60 |
| 3 | 8k x 4k | 40 Mbps | PROJ-EQUI | 60 |

If the quality of the 3rd tier is not acceptable, or you are working with very high motion content, one can lower the resolution and bitrate combination further.

| Tier | Resolution | Bit rate | Projection specifier | fps |
| --- | --- | --- | --- | --- |
| 4 | 5760 x 2880 | 60 Mbps | PROJ-EQUI | 60 |
| 5 | 5760 x 2880 | 40 Mbps | PROJ-EQUI | 60 |
| 6 | 5760 x 2880 | 30 Mbps | PROJ-EQUI | 60 |
| 7 | 4096 x 2048 | 20 Mbps | PROJ-EQUI | 60 |

#### APMP stereoscopic videos:

| Tier | Resolution | Bit rate | Projection specifier | fps |
| --- | --- | --- | --- | --- |
| 1 | 4k x 4k | 80 Mbps | PROJ-HEQU | 60 |
| 2 | 4k x 4k | 60 Mbps | PROJ-HEQU | 60 |
| 3 | 4k x 4k | 40 Mbps | PROJ-HEQU | 60 |

| Tier | Resolution | Bit rate | Projection specifier | fps |
| --- | --- | --- | --- | --- |
| 4 | 2880 x 2880 | 60 Mbps | PROJ-EQUI | 60 |
| 5 | 2880 x 2880 | 40 Mbps | PROJ-EQUI | 60 |
| 6 | 2880 x 2880 | 30 Mbps | PROJ-EQUI | 60 |
| 7 | 2048 x 2048 | 20 Mbps | PROJ-EQUI | 60 |

Following table provides a possible bit rate recommendations for AIV.

| Tier | Average bandwith | Peak bandwidth | Resolution | fps |
| --- | --- | --- | --- | --- |
| 1 | 100 Mbps | 150 Mbps | 4320 x 4320 | 90 |
| 2 | 80 Mbps | 120 Mbps | 4320 x 4320 | 90 |
| 3 | 50 Mbps | 100 Mbps | 4320 x 4320 | 90 |
| 4 | 32 Mbps | 64 Mbps | 4320 x 4320 | 90 |
| 5 | 25 Mbps | 50 Mbps | 4320 x 4320 | 90 |

1.26. For VOD content, the average segment bit rate MUST be within 10% of the `AVERAGE-BANDWIDTH` attribute. (See Declared versus measured values of bandwidths.)

1.27. For VOD content, the measured peak bit rate MUST be within 10% of the `BANDWIDTH` attribute.

1.28. For live (linear) content, the average segment bit rate over a long (~1 hour) period of time MUST be less than 110% of the `AVERAGE-BANDWIDTH` attribute.

1.29. For live (linear) content, the measured peak bit rate MUST be less than 125% of the `BANDWIDTH` attribute.

1.30. For VOD content, the peak bit rate SHOULD be no more than 200% of the average bit rate.

1.31. Different variants MAY have different frame rates.

1.32. \* The default video variants SHOULD be the 2000 kbit/s (average bit rate) variant. (Defaults are the first variant listed in the Multivariant Playlist within a group of variants having compatible audio).

1.33. All video variants SHOULD have identical aspect ratios.

1.34. For maximum compatibility when UHD video resolution is provided, some UHD variants SHOULD be less than or equal to 15 Mbit/s.

1.35. For HDR10 content, the Mastering Display Color Volume and Content Light Level Information SEI messages SHOULD be present.

1.36. MV-HEVC video MUST NOT be used for anything other than stereo video.

1.37. Level for AV1 MUST be less than or equal to Level 6.2

1.38. All APMP monoscopic videos MUST be encoded using HEVC/H.265.

#### Audio

2\. **Audio encoding requirements**

2.1. Audio data SHOULD be provided as an elementary audio stream or in fMP4.

2.2. Codecs that provide stereo audio are:

- Apple Positional Audio Codec (APAC)

- AAC-LC

- HE-AAC v1

- HE-AAC v2

- xHE-AAC

- Apple Lossless

- FLAC

2.3. \* Stereo audio in AAC, HE-AAC v1, or HE-AAC v2 format MUST be provided.

2.4. You SHOULD NOT use HE-AAC if your audio bit rate is above 64 kbit/s.

2.5. Supported multichannel audio codecs are:

- APAC

- Dolby Digital (AC-3)

- Dolby Digital Plus (E-AC-3)(ec-3)

- Dolby Digital Plus JOC (ec+3)

(See Values for the CODECS attribute for more information about specifying Dolby Digital Plus JOC.)

2.6. \* If Dolby Digital Plus is provided and your streams are delivered to devices that don’t support Dolby Digital Plus, then Dolby Digital MUST be provided also. See Audio compatibility.

2.7. Stereo audio MAY be provided at multiple bit rates.

2.8. \* Multichannel audio using a particular codec MAY be provided at multiple bit rates.

2.9. Overall bit rate recommendations are as follows:

#### Bitrate recommendations for stereo are as follows:

| Audio channels | Codec | Total (kbit/s) |
| --- | --- | --- |
| 2.0 (stereo) | APAC | 32 to 160 |
| 2.0 (stereo) | AAC | 32 to 160 |
| 2.0 (stereo) | xHE-AAC | 24 to 160 |
| 2.0 (stereo) | Dolby Digital Plus | 96 to 160 |

#### Bitrate recommendations for multi-channel surround formats are as follows:

| Audio channels | Codec | Total (kbit/s) |
| --- | --- | --- |
| 5.1 (surround) | APAC | 320 |
| 5.1 (surround) | AAC | 320 |
| 5.1 (surround) | Dolby Digital | 384 |
| 5.1 (surround) | Dolby Digital Plus | 192 |
| 7.1 (surround) | APAC | 384 |
| 7.1 (surround) | Dolby Digital Plus | 384 |

#### Bitrate recommendations for Ambisonics (https://developer.apple.com/av-foundation/Apple-Positional-Audio-Codec.pdf) are as follows:

| Ambisonic order | Codec | Audio coding identifier | Total (kbit/s) |
| --- | --- | --- | --- |
| 1 | APAC | 1OA | 192 to 384 |
| 2 | APAC | 2OA | 240 to 512 |
| 3 | APAC | 3OA | /270 to 768 |

2.10. \* You MAY change channel layout within a stream.

2.11. Channel layout changes MUST be in conjunction with an `EXT-X-DISCONTINUITY` tag.

2.12. If you provide Descriptive Video Service (DVS), also called “Audio Description”, it MUST be marked with the attribute `CHARACTERISTICS="public.accessibility.describes-video"`.

2.13. If you provide DVS, the `AUTOSELECT` attribute MUST have a value of “ `YES"`.

2.14. The name of DVS audio SHOULD indicate that the stream is DVS content.

2.15. If you provide alternative audio or DVS, you MUST provide it for the entire content duration, even if it only really exists for a portion of the main content.

2.16. Alternative audio or DVS MAY reuse the audio segments of regular content when the alternative content isn’t available.

2.17. A single Media Segment MUST NOT contain multiple audio streams.

2.18. Loudness management or Dynamic range control SHOULD be present unless all content (including ads) has been encoded at the same audio levels.

2.19. In fMP4 files, except for the APAC codec, you SHOULD provide loudness information by way of a loudness box (’ `ludt`’). When present, the loudness box takes precedence over any loudness information in the audio stream. For APAC, a loudness box SHALL not be used.

2.20. In the absence of a loudness box, Dolby Digital and Dolby Digital Plus loudness SHOULD be specified by the `dialnorm` field (ATSC A/52:2012).

2.21. For AAC, in the absence of a loudness box, AAC dialog loudness SHOULD be specified by either AAC `prog_ref_level` (ISO 14496-3 subclause 4.5.2.7), as specified by SCTE 193-1 section 7.4.1, or by the `loudnessInfo()` payload as specified by ISO 23003-4, in which case, `samplePeakLevel` or `truePeakLevel` MUST be present, `measurementSystem` MUST be 2, and `methodDefinition` MUST be 1 or 2, while for video content it SHOULD be 2.

2.22. For xHE-AAC, loudness metadata MUST be present according to the Basic Loudness Metadata specified in ISO 23003-4 Table I.5; `samplePeakLevel` or `truePeakLevel` MUST be present. The `methodDefinition` SHOULD be 2 for video content.

2.23. The loudness value MUST indicate the actual loudness of the content.

2.24. HE-AAC in fMP4 files MUST use explicit signaling of SBR data.

2.25. The container format for xHE-AAC, Apple Lossless, FLAC, and APAC audio MUST be fMP4.

2.26. If you provide non-Dolby multichannel audio, you SHOULD provide multichannel AAC also.

2.27. For audio description, the LANGUAGE attribute MUST be present and indicate the primary language used to convey the descriptions.

2.28. Audio that has been prepared or otherwise processed to heighten the intelligibility of speech MAY be marked with the attribute `CHARACTERISTICS="public.accessibility.enhances-speech-intelligibility"`.

2.29. Supported multi-format audio codecs that carry the combination of two or more formats out of channels, objects and Ambisonics are:

2.30. APAC encoded content MUST have in-stream loudness and DRC metadata.

2.31. If you provide APAC immersive audio, you SHOULD provide stereo AAC also.

#### Ads and pre-/mid-/post-rolls

3\. **Ad requirements** (See also the Media Playlists section of HTTP Live Streaming (HLS) authoring specification for Apple devices.)

3.1. Your ads and other nonprimary media MAY be inserted in the Media Playlists or as Interstitials.

3.2. Inserted media SHOULD be encoded with the same codecs as the other content in the Media Playlist.

3.3. Inserted media SHOULD be encoded with the same aspect ratio as the other content in the Media Playlist.

3.4. Inserted media SHOULD be at or under the specified bandwidths for that variant.

#### Accessibility

4\. **Accessibility requirements**

4.1. Captions SHOULD be provided with your streams to make content accessible to people who are deaf or hard of hearing.

4.2. Supported caption formats are:

- CEA-608 closed captions

- CEA-708 closed captions

- WebVTT subtitles

- IMSC1 subtitles (text profile only)

4.3. Closed captions (if any) MUST be included in the video Media Segments.

4.4. The presence of closed captions MUST be declared via an `EXT-X-MEDIA` tag that contains a `LANGUAGE` attribute.

4.5. If a subtitles track is intended to provide accessibility for people who are deaf or hard of hearing, it MUST be marked with the attribute `CHARACTERISTICS="public.accessibility.transcribes-spoken-dialog,public.accessibility.describes-music-and-sound"`. (Subtitles with this attribute value are treated the same as closed captions.)

4.6. If a subtitles track is intended to provide accessibility for people who are deaf or hard of hearing, the `AUTOSELECT` attribute MUST have a value of `"YES"`.

4.7. The `LANGUAGE` attribute MUST be included in the `EXT-X-MEDIA` tag for a subtitles track.

4.8. For information on including audio descriptions with your streams, see items 2.12 through 2.16.

#### Subtitles

5\. **Subtitle requirements**

5.1. Subtitles MAY be provided.

5.2. \* Subtitles MUST be WebVTT (according to the HLS specification) or IMSC1 in fMP4.

5.3. WebVTT subtitles MUST be in text files, with an `X-TIMESTAMP-MAP` according to the HLS specification.

5.4. IMSC1 subtitles MUST be in fMP4 files.

5.5. The subtitle playlist MUST exist for the entirety of the main content, even if the actual subtitles only exist for a portion of the content.

5.6. For live (linear) content, target durations for subtitle playlists MUST be identical to other media.

5.7. For VOD content, target durations of subtitle playlists MAY be longer than the other media.

5.8. If the content has forced subtitles and regular subtitles in a given language, the regular subtitles track in that language MUST contain both the forced subtitles and the regular subtitles for that language.

5.9. If your videos contain text burnt into the video and you have access to a version without the burn-in, you SHOULD use forced subtitles instead. (This allows you to easily translate into multiple languages. An example of when you might use forced subtitles is a science fiction film, where alien languages are translated into English.)

5.10. The kind of subtitles SHOULD be specified in the `CODECS` attribute of the associated `EXT-X-STREAM-INF` tags. You SHOULD use `"stpp.ttml.im1t"` to identify IMSC1 subtitles. You MAY use `"wvtt"` to identify WebVTT subtitles.

5.11. Forced subtitles SHOULD always have `AUTOSELECT=YES`.

#### Trick Play

6\. **Trick play requirements**

6.1. I-frame playlists ( `EXT-X-I-FRAME-STREAM-INF`) MUST be provided to support scrubbing and scanning UI.

6.2. You SHOULD have one frame per second _dense_ I-frame renditions. These are dedicated renditions that only contain I-frames.

6.3. Alternatively, you MAY use the I-frames from your normal content, but trick play performance is improved with a higher density of I-frames.

6.4. If you provide multiple bit rates at the same spatial resolution for your regular video, you SHOULD create the I-frame playlist for that resolution from the same source used for the lowest bit rate in that group.

6.5. The bit rate of I-frame playlists SHOULD be the bit rate of a normal playlist of the same resolution times the fps of the I-frame playlist divided by eight. (See I-frame bit rates versus normal bit rates.)

6.6. \* You SHOULD provide multiple I-frame Media Playlists with different bit rates.

6.7. As with normal video, there are many possible choices of bit rates for dense I-frame variants. The following tables provide one possible set of variants. (See On bit rates for variants.)

| 16:9 aspect ratio | H.264/AVC |
| --- | --- |
| 640 x 360 | 45 |
| 768 x 432 | 90 |
| 960 x 540 | 250 |
| 1280 x 720 | 375 |
| 1920 x 1080 | 580 |

| 16:9 aspect ratio | HEVC/H.265 | HDR (HEVC) |
| --- | --- | --- |
| 768 x 432 | 40 | 55 |
| 960 x 540 | 75 | 94 |
| 960 x 540 | 200 | 238 |
| 1280 x 720 | 300 | 360 |
| 1920 x 1080 | 525 | 650 |

6.8. I-frame playlists MUST contain the `EXT-X-I-FRAMES-ONLY` tag.

6.9. The peak segment bit rate MUST be calculated according to the HLS specification.

6.10. If using fMP4, I-frame segments MUST include the ‘moof’ header associated with the I-frame.

6.11. For live (linear) content, target durations for I-frame playlists MUST be identical to other media.

6.12. For VOD content, target durations of I-frame playlists MAY be different from the other media.

6.13. \* I-frame playlists MAY use a different video codec than the normal video segments.

6.14. \* For backward compatibility, some trick play content SHOULD be encoded with H.264.

6.15. If HDR trick play streams are provided, they SHOULD be provided at all resolutions.

6.16. \* For backward compatibility, SDR trick play streams MUST be provided.

6.17. I-frame content MAY be encoded using the fMP4 ‘mjpg’ codec. (See I-frame image sequences.)

#### Media Segmentation

7\. **Media segmentation requirements**

7.1. Your media MUST be continuous across segments, with the exception of transitions for ads and other inserted material.

7.2. If using a transport stream, continuity counters and timestamps MUST be sequential.

7.3. If using fMP4, the track fragment decode time MUST be consistent with the decode time and duration of the previous segment.

7.4. Video segments MUST start with an IDR frame.

7.5. Target durations SHOULD be 6 seconds.

7.6. Segment durations SHOULD be nominally 6 seconds (for example, NTSC 29.97 may be 6.006 seconds).

7.7. Media Segments MUST NOT exceed the target duration by more than 0.5 seconds.

7.8. Each xHE-AAC segment SHOULD start with an Immediate Playout Frame (IPF).

7.9. Each APAC segment MUST start with an Audio Synchronization Packet (ASP).

#### Media Playlists

8\. **Media Playlist requirements**

8.1. You MUST use sufficiently accurate segment durations to ensure that the sum of the `EXTINF` durations of any contiguous group of segments is within one video frame duration of the actual duration of the content.

8.2. Audio and video playlists MUST all use the same target duration.

8.3. Audio and video playlists MUST contain the same duration of the content.

8.4. The `EXT-X-PROGRAM-DATE-TIME` tag MUST be present in every live (linear) Media Playlist.

8.5. The date-time value of an `EXT-X-PROGRAM-DATE-TIME` tag SHOULD be aligned with the airtime of the content.

8.6. If your Media Playlists are created from static source content (VOD), you MUST add the `EXT-X-PLAYLIST-TYPE` with the value `VOD`.

8.7. Within one asset, all Media Playlists with an `EXT-X-PLAYLIST-TYPE` of `VOD` MUST cover exactly the same media time range.

8.8. If your Media Playlists are event style (start from a fixed point with segments never removed), you MUST add the `EXT-X-PLAYLIST-TYPE` with the value `EVENT`.

8.9. Separate audio streams MUST be declared using `EXT-X-MEDIA` tags.

8.10. The `LANGUAGE` attribute MUST be included in every `EXT-X-MEDIA` tag that doesn’t have `TYPE=VIDEO`.

8.11. You MUST provide at least six segments in a live (linear) playlist.

8.12. \* You SHOULD provide at least 15 minutes of content in a live (linear) playlist.

8.13. Breaks of encoding continuity MUST be indicated with the `EXT-X-DISCONTINUITY` tag.

8.14. Video frame rate changes MUST be marked as a discontinuity using `EXT-X-DISCONTINUITY` tags.

8.15. All variants and renditions MUST have discontinuities at the same points in time.

8.16. \* You SHOULD avoid switching codecs at discontinuities, for example, switching between HEVC and H.264, or between AAC and Dolby Digital.

8.17. If live (linear) content will ever contain an `EXT-X-DISCONTINUITY` tag, the `EXT-X-DISCONTINUITY-SEQUENCE` tag MUST always be present.

8.18. Your media requests MUST NOT use HTTP redirects, with the exception of ad content to allow dynamic selection of ads.

8.19. You SHOULD identify interstitial and program boundaries using the `EXT-X-DATERANGE` tag.

8.20. If using fMP4, `EXT-X-MAP` tags MUST be present.

8.21. Metadata SHOULD be in the playlist (using `EXT-X-DATERANGE`) rather than in the media (using Timed Metadata).

8.22. \* For maximum interoperability, all audio/video variants and renditions SHOULD have segment boundaries at the same points in time.

8.23. If your xHE-AAC segments start with an IPF, you SHOULD use the `EXT-X-INDEPENDENT-SEGMENTS` tag in the Media Playlist.

8.24. A live (linear) playlist update SHOULD be considered invalid when the Last-Modified HTTP header, if supplied, is more than three target durations from the Date HTTP header.

8.25. If your APAC segments start with an ASP, you SHOULD use the `EXT-X-INDEPENDENT-SEGMENTS` tag in the Media Playlist.

#### Multivariant Playlist

9\. **Multivariant Playlist requirements**

9.1. Your `EXT-X-STREAM-INF` tag MUST always provide the `CODECS` attribute.

9.2. Your `EXT-X-STREAM-INF` tag MUST always provide the `RESOLUTION` attribute if the rendition includes video.

9.3. Your `EXT-X-I-FRAME-STREAM-INF` tag MUST always provide the `CODECS` attribute.

9.4. Your `EXT-X-I-FRAME-STREAM-INF` tag MUST always provide the `RESOLUTION` attribute.

9.5. You SHOULD deliver video and audio as separate streams.

9.6. If you have multichannel audio, you MUST use separate audio streams.

9.7. If you have alternative audio content (languages/commentary/DVS), you MUST use separate audio streams.

9.8. If you have different video angles, you MUST use separate audio streams.

9.9. You MUST provide multiple bit rates of video (that is, variants).

9.10. For HD content, there SHOULD be at least two variants encoded at the highest-available resolution.

9.11. If your video segments start with an IDR, you SHOULD use the `EXT-X-INDEPENDENT-SEGMENTS` tag in the Multivariant Playlist. (See item 7.4.)

9.12. If your video segments start with an IDR and the `EXT-X-INDEPENDENT-SEGMENTS` tag isn’t in the Multivariant Playlist, you MUST use the `EXT-X-INDEPENDENT-SEGMENTS` tag in all video Media Playlists. (See item 7.4.)

9.13. The `BANDWIDTH` attribute MUST be the largest sum of peak segment bit rates that’s produced by any playable combination of renditions.

9.14. You MUST include the `AVERAGE-BANDWIDTH` attribute.

9.15. Each `EXT-X-STREAM-INF` tag that includes video content MUST have a `FRAME-RATE` attribute.

9.16. The `VIDEO-RANGE` attribute MUST be specified unless all variants and renditions are SDR.

9.17. Within a group of Renditions ( `EXT-X-MEDIA` tags having the same `TYPE` and `GROUP-ID`), those tags having the same `LANGUAGE` value should be ordered from most general to most specific. (Because `CHARACTERISTICS` are open-ended, the matching algorithm needs the ordering since it can’t interpret all the semantics.)

9.18. An `EXT-X-CONTENT-STEERING` tag SHOULD always have a `PATHWAY-ID` attribute.

9.19. The `SCORE` attribute (if present) MUST be on every variant. Otherwise, the `SCORE` attribute will be ignored.

9.20. For APAC, the APAC profile and level MUST be provided as a part of Codec string. See \[APAC\] (https://developer.apple.com/av-foundation/Apple-Positional-Audio-Codec.pdf) for more information about APAC profile and level.

#### Delivery

10\. **Delivery requirements**

10.1. The server MUST deliver playlists using `gzip` content-encoding.

10.2. You SHOULD support stream failover, for example by listing duplicate streams in the Multivariant Playlist.

10.3. Media data SHOULD NOT be delivered to the application through a local server.

10.4. You SHOULD use the recommended MIME types for content. The recommendations are in the following table:

| Media type | Format | Recommended MIME type | Typical file extension |
| --- | --- | --- | --- |
| Playlist | HLS playlist | `application/vnd.apple.mpegurl` | `m3u8` |
| Playlist | M3U playlist | `audio/mpegurl` | `m3u` |
| Video | MPEG transport stream | `video/mp2t` | `ts` |
| Media Initializaton | Fragmented MP4 | `video/mp4` | mp4 |
| Video or audio | Fragmented MP4 | `video/iso.segment` | m4s |
| Video | Fragmented MP4 | `video/mp4` | `mp4` |
| Audio | MPEG transport stream | `video/mp2t` | `ts` |
| Audio | Fragmented MP4 | `audio/mp4` | `mp4` |
| Audio | Packed audio | `audio/aac` | `aac` |
| Audio | Packed audio | `audio/mpeg` | `mp3` |
| Audio | Packed audio | `audio/ac3` | `ac3` |
| Audio | Packed audio | `audio/eac3` | `ec3` |
| Subtitles | WebVTT | `text/vtt` or `text/plain` | `vtt` |
| Subtitles | IMSC1 | `application/mp4` | `mp4` |
| Content Steering Manifest | JSON file | `application/vnd.apple.steering-list` | json |
| `X-ASSET-LIST` response | JSON file | `application/json` | json |

#### Privacy

11\. **Privacy requirements**

11.1. Multivariant Playlists SHOULD be delivered using Transport Layer Security (TLS).

11.2. Media Playlists SHOULD be delivered using TLS.

11.3. Media Segments SHOULD be delivered using TLS.

11.4. Media Segment URLs requested over unencrypted transport SHOULD NOT contain revealing strings, such as movie title, show title, episode name, episode number, genre, advertiser, or product.

#### Security

12\. **Security requirements**

12.1. Transport Layer Security (TLS) MUST be version 1.2 or later with forward secrecy.

12.2. TLS MUST NOT use known-insecure cryptographic primitives (such as, RC4 encryption, SHA-1 certificate signatures).

12.3. Within TLS, key sizes MUST be 2048 bits for RSA and 256 bits for EC.

12.4. The URLs for Media Segments SHOULD NOT be completely static. URLs should be issued per device or changed over time.

#### Content Protection

13\. **Content protection requirements**

13.1. Content protection of video and audio SHOULD follow the FairPlay Streaming (FPS) specification.

13.2. If the content is encrypted with FPS, the method MUST be `SAMPLE-AES`.

13.3. If the content is encrypted with FPS, the key format MUST be `"com.apple.streamingkeydelivery"`.

13.4. The `IV` attribute SHOULD NOT be used with FPS unless necessary for interoperability.

13.5. Content with `HD` resolutions SHOULD use `HDCP-LEVEL` of `TYPE-0`.

13.6. Content with greater than `HD` resolutions SHOULD use `HDCP-LEVEL` of `TYPE-1`.

13.7. Video encrypted with Common Encryption MUST use an `encrypt:skip` pattern of 1:9 (10% partial encryption).

13.8. Content encrypted with FPS MAY use the `ALLOWED-CPC` attribute. (See ALLOWED-CPC values for FairPlay Streaming.)

13.9. Common encryption MUST NOT use content sensitive encryption.

13.10. Content authors MAY mix encrypted and unencrypted samples in a single HLS fMP4 segment with a single Media Initialization Section by supplying both an encrypted SampleDescription at index 0 and an unencrypted SampleDescription at index 1 for each track. The sample index field of each sample should point to the appropriate SampleDescription.

13.11. Encryption with `SAMPLE-AES-CTR` SHALL NOT be used on Apple devices.

#### Low-Latency HLS

14\. **Low-Latency HLS requirements**

14.1. Low-Latency stream delivery MUST meet all requirements of the Low-Latency Server Configuration Profile in Appendix B of draft-pantos-hls-rfc8216bis-07 or later.

14.2.

14.2a. The Part Target Duration MUST be at least the maximum round-trip time (RTT) to the server that 95% of the clients are expected to see (P95 RTT).

14.2b. The Part Target Duration SHOULD be at least three times the P95 RTT.

14.2c. The RECOMMENDED Part Target Duration is one second.

14.3. The `PART-HOLD-BACK` value MUST be at least three times the Part Target Duration.

14.4. Services with Playlist windows longer than two minutes SHOULD offer Playlist Delta Updates.

14.5. Services that offer Playlist Delta Updates and use `EXT-X-DATERANGE` tags SHOULD also use `CAN-SKIP-DATERANGES=YES`.

#### SharePlay

15\. **SharePlay HLS requirements**

15.1. For live (linear) content, the timeline derived from the EXT-X-PROGRAM-DATE-TIME tag is used for synchronization. That timeline MUST be in agreement for all participants.

15.2. For VOD content, the timeline based on the start of the playlist is used for synchronization. That timeline MUST be in agreement for all participants.

15.3. Interstitials delivered to participants in a SharePlay session SHOULD match in duration. If they do not, participants receiving longer duration interstitials will miss some of the primary content. This behavior can only be overridden when all participants are using apps that support control of coordinated media playback.

#### Spatial (stereo, immersive and projected) video

16\. **Spatial (stereo, immersive and projected) video requirements**

16.1. All variants containing spatial video MUST be marked with a REQ-VIDEO-LAYOUT attribute.

16.2. All spatial video content MUST include Video Extended Usage ( `'vexu'`) atoms/boxes. (See Additional spatial video specifications.)

16.3. Switches between spatial and non-spatial video content MUST be marked with an EXT-X-DISCONTINUITY tag, or the Media Initialization Section MUST contain sample descriptions for both kinds of content.

16.4. Stereo and Immersive video content SHOULD include parallax metadata if your content has subtitles. (See Additional spatial video specifications.)

16.5. If spatial video content includes sections of monoscopic video content, then the REQ-VIDEO-LAYOUT attribute MUST include “CH-MONO” as one entry.

### Amended requirements for macOS

All general rules apply except as expressly modified by a rule with the same number in this section. Rules with a leading plus sign (+) are additional rules.

#### Video

1.3b. Profile and Level for H.264 MUST be less than or equal to High Profile, Level 5.0.

### Amended requirements for iOS

#### Video

1.6b. Profile and Level for H.264 MUST be less than or equal to High Profile, Level 6.0.

1.9.

1.9a. Profile and Level for Dolby Vision MUST be Profile 5 (single layer 10-bit HEVC) or Profile 10 (single layer 10-bit AV1) and less than or equal to Level 9.

1.9b. + For maximum compatibility, some Dolby Vision variants SHOULD be Profile 5 and less than or equal to Level 7.

1.32.

1.32a. For Wi-Fi delivery, the default video variant SHOULD be the 2000 kbit/s (average bit rate) variant.

1.32b. For cellular delivery, the default video variant SHOULD be the 730 kbit/s (average bit rate) variant.

#### Multivariant Playlist

9.21. + Multivariant Playlists that are delivered over cellular networks MUST contain a variant whose peak `BANDWIDTH` is less than or equal to 192 kbit/s.

9.22. + For backward compatibility, a peak 192 kbit/s H.264 variant packaged in a transport stream SHOULD be provided for cellular.

### Amended requirements for visionOS

The following general rules regarding compatibility aren’t applicable in visionOS if all variants contain stereo video content: 1.3a, 1.6a, 1.9b, 1.12, 1.24, 2.3, 2.6, 6.14, 6.16.

#### Video

1.9a. Dolby Vision monoscopic content MUST be Profile 5 (single layer 10-bit HEVC) and less than or equal to Level 9.

1.9c. + Dolby Vision stereo video MUST be Profile 20 (MV-HEVC) and less than or equal to Level 9.

1.25. Suggested bit rates for MV-HEVC variants.

| 16:9 aspect ratio | MV-HEVC SDR 30 fps | MV-HEVC HDR 30 fps | Frame rate |
| --- | --- | --- | --- |
| 640 x 360 | 246 | 272 | ≤ 30 fps |
| 768 x 432 | 510 | 612 | ≤ 30 fps |
| 960 x 540 | 1020 | 1241 | ≤ 30 fps |
| 960 x 540 | 1530 | 1853 | ≤ 30 fps |
| 960 x 540 | 2720 | 3281 | Same as source |
| 1280 x 720 | 4080 | 4930 | Same as source |
| 1280 x 720 | 5780 | 6936 | Same as source |
| 1920 x 1080 | 7650 | 9180 | Same as source |
| 1920 x 1080 | 9660 | 11900 | Same as source |
| 2560 x 1440 | 13770 | 16490 | Same as source |
| 3840 x 2160 | 19720 | 23630 | Same as source |
| 3840 x 2160 | 28560 | 34000 | Same as source |

1.39. + Stereo video MUST be encoded using Dolby Vision Profile 20 (MV-HEVC).

#### Trick play

6.6. If your only content is stereo video, then you SHOULD provide only one I-frame Media Playlist. (See item 6.19.)

6.18. + Trick play content SHOULD be monoscopic and rectilinear.

6.19. + In visionOS, a thumbnail list is produced for scrubbing and scanning. These thumbnails are 160px height with a width that matches the aspect ratio of the main content. For better performance, you MAY provide an I-frame playlist having exactly this height.

#### Spatial (stereo, immersive and projected) video

16.6. + All Stereo (including APMP) video MUST be encoded using MV-HEVC.

16.7. + Immersive video content MUST use CH-STEREO and PROJ-AIV for channel and projection specifier in REQ-VIDEO-LAYOUT.

### Amended requirements for tvOS

#### Video

1.3b. Profile and Level for H.264 MUST be less than or equal to High Profile, Level 5.1.

1.20. For HDR content, frame rates less than or equal to 30 fps MUST be provided.

1.25. The 145 kbit/s variant SHOULD NOT be provided.

#### Audio

2\. Audio encoding requirements

2.8. Multichannel audio using a particular codec MAY be provided at multiple bit rates. However, Dolby Atmos content SHOULD be restricted to a single bit rate.

#### Trick Play

6.16. SDR trick play streams MUST be provided.

#### Media Playlists

8.12. You SHOULD provide at least 120 minutes of content in a live (linear) playlist.

#### Multivariant Playlist

9.20. + You MUST have no audio-only variants listed in the Multivariant Playlist.

### Amended requirements for AirPlay 2-Enabled TVs

#### Video

1.23. If multiple video streams are provided (H.264, HEVC, HDR), each stream MUST provide all anticipated bandwidths.

1.39. + Encrypted fMP4 content MUST contain either a Sample Encryption Box ( `'senc'`), or both a Sample Auxiliary Information Sizes Box ( `'saiz'`) and a Sample Auxiliary Information Offsets Box ( `'saio'`).

#### Audio

2.10. Channel layout SHOULD NOT change within a stream.

#### Ads and pre-/mid-/post-rolls

3\. **Ad requirements**

3.5. + Inserted media SHOULD be at a similar frame rate (x, 2x, x/2) as the other content in the Media Playlist.

#### Subtitles

5.2. Subtitles MUST be WebVTT.

#### Trick Play

6.13. If a normal video variant uses a video codec, one or more I-frame variants MUST exist with the same video codec or the `mjpg` codec.

#### Media Playlists

8.16. You SHOULD NOT switch codecs at discontinuities. For example, don’t switch between HEVC and H.264, or between AAC and Dolby Digital.

8.22. All video variants and renditions MUST have segment boundaries at the same points in time.

8.25. + Frame rate changes at discontinuities SHOULD use a similar frame rate (x, 2x, x/2).

#### Multivariant Playlist

9.23. + You SHOULD provide a full range of variants for each codec type and frame rate. Similar frame rates (x, 2x, x/2) are compatible, nonsimilar frame rates may cause playback issues.

9.24. + If you supply HDR content, you SHOULD provide both Dolby Vision and HDR10.

### Revision history

The following table describes the changes to this document.

| Date | Notes |
| --- | --- |
| 2025-05-08 | Added AIV bit-rate tiers. |
| 2025-05-02 | Added Offline download guidelines. |
| 2025-04-30 | Added APAC authoring guidelines. |
| 2025-04-18 | Added Spatial (Stereo, APMP and AIV) authoring guidelines. |
| 2025-03-25 | Clarified use of DV20 for Stereo video for VisionOS. |
| 2023-05-24 | Minor changes. |
| 2023-08-15 | Added visionOS requirements. Added note about audio/aac. |
| 2023-06-27 | Added stereo video rules and MV-HEVC bit rate. |
| 2023-05-19 | Added detail about I-frame image sequences. |
| 2022-08-22 | Added “Audio rendition groups and variants” section to the appendix, clarified language around the LANGUAGE attribute, and added additional information about Apple TV and Dolby ATMOS. |
| 2021-11-12 | Renamed “primary playlist” to “Multivariant Playlist.” |
| 2020-06-22 | Added new sections: Low-Latency HLS and ALLOWED-CPC Values for FairPlay Streaming. |
| 2019-06-03 | Added new table describing MIME types. |
| 2019-03-04 | Added new rules for Airplay 2-enabled TVs. Moved appendixes into child article. |
| 2018-09-11 | Added new rules for content protection and media playlists. |
| 2018-06-18 | Added Dolby Digital Plus with Dolby Atmos information. Added codec value section. |
| 2018-04-09 | Made several minor changes to individual spec points. Updated the variant bit rate table and broke it into two separate tables. |
| 2018-01-16 | Fixed several typos and made a couple of minor changes to audio encoding requirements. |
| 2017-09-19 | Updated document with HDR (HEVC) information. |
| 2017-06-06 | Updated document with HEVC/H.265 information. |
| 2016-09-13 | Added rules for fragmented MP4 files. |
| 2016-06-13 | Updated for iOS and macOS specifications. |
| 2016-03-21 | Updated Dolby Digital bit rate recommendation to 384 kbit/s. |
| 2016-01-11 | Fixed typo in section 10.2. |
| 2015-12-17 | Added section on using the `hlsreport` tool. |
| 2015-12-08 | Corrected a mistake in Table 2-3, Column 2 heading. Changed to 16:9 aspect from 19:0. |
| 2015-10-21 | Published the first edition of this document describing the HTTP Live Streaming specifications for audio and video content delivery for Apple TV. |

## Topics

### Appendixes

HTTP Live Streaming (HLS) Authoring Specification for Apple devices appendixes

Learn additional information related to the HLS Authoring Specification for Apple Devices.

## See Also

### Specifications and other documents

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/using-content-protection-systems-with-hls

- HTTP Live Streaming
- Using content protection systems with HLS

Article

# Using content protection systems with HLS

Adding encryption keys to media playlists

## Overview

HTTP Live Streaming (HLS) supports content protection systems through the presence of `EXT-X-KEY` tags in playlists. HLS allows multiple `EXT-X-KEY` tags with diﬀerent `KEYFORMAT` attributes to apply to the same segments provided that each of the tags ultimately produces the same decryption key. This is necessary because you can only encrypt a media segment with one encryption method, using one encryption key, with a single IV (initialization vector).

While a playlist may contain `EXT-X-KEY` tags for more than one protection system, a player typically supports only one protection system. This means that every encrypted segment must have `EXT-X-KEY` tags for the same set of protection systems. The player refuses to play the playlist if it doesn’t handle any of the protection systems. If the player can handle more than one protection system, it chooses one. The playlist has no mechanism to convey a preference for a protection system.

This document provides general guidance on using such `EXT-X-KEY` tags.

For convenience sake, this document refers to some details of the Google Widevine and Microsoft PlayReady protection systems. The documentation for those systems should be used to ensure accurate implementation.

## Set the playlist key tag

The `EXT-X-KEY` tag has three attributes that principally control its behavior. These are `METHOD`, `KEYFORMAT`, and `URI`.

`METHOD`

Apple’s HLS encryption uses the AES block cipher algorithm and Cipher Block Chaining (CBC) mode. To guarantee compatibility with FairPlay, you must use the `METHOD=SAMPLE-AES`. In terms of the Common Encryption standard (ISO/IEC 23001-7), this is the `cbcs` protection scheme. If FairPlay isn’t involved you may use another `METHOD`.

`KEYFORMAT`

Use this attribute to convey how to obtain the key. For more information, see Choose a key format for more detail. This can be modified by the attribute `KEYFORMATVERSIONS`. However, in most cases, this additional attribute should be either left oﬀ or set to the string value `"1"`.

`URI`

This contains the information needed to identify the specific key. The format of the `URI` is determined by the `KEYFORMAT` value.

## Choose a key format

There are four supported key formats:

- Identity

- FairPlay Streaming

- Widevine

- PlayReady

All formats (except Identity) require a key server. That is, a server that uses some protocol to supply the keys. The key server isn’t specified by the playlist. Instead, the playback app is responsible for knowing the URI of the key server and the protocol for communicating with that server.

### Identity

This format is identified by a `KEYFORMAT` attribute with the value `identity` or by the lack of a `KEYFORMAT` attribute.

The `URI` attribute is the URI of the key file.

Because there is no key server involved, this protection system aﬀords only a minimal level of protection. For that reason you shouldn’t use identity keys in conjunction with any other protection system.

This format is described in HTTP Live Streaming 2nd Edition

### FairPlay Streaming

This format is identified by a `KEYFORMAT` attribute with the value `com.apple.streamingkeydelivery`.

Further details about FairPlay Streaming are available at FairPlay Streaming.

### Widevine

The Widevine format has more than one version. However, the versions use diﬀerent key format values; from the HLS point of view, they are completely distinct. You should use what the Widevine documentation refers to as v2.

This key format is identified by a `KEYFORMAT` attribute with the value `urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed`. (The UUID in this URN is the Widevine System ID. See Widevine PSSH data.)

For more information about Widevine refer to Widevine Technologies.

### PlayReady

The PlayReady format is defined by Microsoft.

This key format is identified by a `KEYFORMAT` attribute with the value `com.microsoft.playready`.

For more information refer to the PlayReady documentation.

## Select key identifiers

All three of the key formats that use a key server - FairPlay Streaming, Widevine, PlayReady - contain something called a key identifier. The key identifier is the data sent to the server so it can return the correct key.

The FairPlay Streaming key identifier has no relationship to that used by the other formats.

The Widevine and PlayReady key identifiers may be identical. Their value should be a UUID. Note that PlayReady does not store the UUID as a simple 16-byte array. (See the Example below for more detail.)

## Create a PSSH box

The Protection System Specific Header (‘pssh’) box is defined in ISO/IEC 23001-7.

This is an ISO Base Media File Format (MP4) structure used to convey information about the protection system. It’s only necessary with Widevine and PlayReady. If you use those protection systems, you should include a PSSH box for each system you use in the media initialization sections of your stream.

The following is the layout of the version 0 PSSH box.

PSSH box {
UInt32 size // Length of the whole box
UInt32 type // == ‘pssh’
UInt32 version_and_flags // == 0
UInt8 SystemID[16]
UInt32 DataSize
UInt8 Data[DataSize] // System specific data
}

The `SystemID` is a UUID that indicates how to parse the `Data` portion of the PSSH.

### Widevine PSSH data

The Widevine `SystemID` is `edef8ba9-79d6-4ace-a3c8-27dcd51d21ed`.

The `Data` field contains a protocol buﬀer (that is, a mechanism for serializing structured data; see Protocol Buffers).

The Widevine documentation details the specific messages that are possible.

The data will contain the key identifier and the protection scheme.

### PlayReady PSSH data

The PlayReady `SystemID` is `9a04f079-9840-4286-ab92-e65be0885f95`.

The `Data` field is PlayReady Object that contains a PlayReady Header.

The PlayReady Object is a binary data structure that contains one or more PlayReady Object Records. Each record has a type; one of these types is a PlayReady Header.

The PlayReady Header is a little-endian UTF-16 XML string. This contains the header version, protection scheme, and key identifier. You should use the header version `v4.3.0.0` as this is necessary to support the ‘cbcs’ protection scheme.

## Example

Here is an example of FairPlay Streaming, Widevine, and PlayReady keys.

#EXT-X-KEY:METHOD=SAMPLE-AES,URI="data:text/plain;charset=UTF-16;base64,vgEAAAEAAQC0ATwAVwBSAE0ASABFAEEARABFAFIAIAB4AG0AbABuAHMAPQAiAGgAdAB0AHAAOgAvAC8AcwBjAGgAZQBtAGEAcwAuAG0AaQBjAHIAbwBzAG8AZgB0AC4AYwBvAG0ALwBEAFIATQAvADIAMAAwADcALwAwADMALwBQAGwAYQB5AFIAZQBhAGQAeQBIAGUAYQBkAGUAcgAiACAAdgBlAHIAcwBpAG8AbgA9ACIANAAuADMALgAwAC4AMAAiAD4APABEAEEAVABBAD4APABQAFIATwBUAEUAQwBUAEkATgBGAE8APgA8AEsASQBEAFMAPgA8AEsASQBEACAAQQBMAEcASQBEAD0AIgBBAEUAUwBDAEIAQwAiACAAVgBBAEwAVQBFAD0AIgBOAEMAUQBVAEIARgBSAEUAZABHAFMARQBsAEsAUwAwAHgATgBUAGsAOQBBAD0APQAiAD4APAAvAEsASQBEAD4APAAvAEsASQBEAFMAPgA8AC8AUABSAE8AVABFAEMAVABJAE4ARgBPAD4APAAvAEQAQQBUAEEAPgA8AC8AVwBSAE0ASABFAEEARABFAFIAPgA=",KEYFORMAT="com.microsoft.playready",KEYFORMATVERSIONS="1"

### FairPlay

The FairPlay Streaming URI value, except for the URL scheme prefix, is the key identifier.

### Widevine

Here is the unpacked form of the Widevine base64 string (a PSSH box).

00000000 00 00 00 38 70 73 73 68 00 00 00 00 ed ef 8b a9 |...8pssh........|
00000010 79 d6 4a ce a3 c8 27 dc d5 1d 21 ed 00 00 00 18 |y.J...'...!.....|
00000020 12 10 04 14 24 34 44 54 64 74 84 94 a4 b4 c4 d4 |....$4DTdt......|
00000030 e4 f4 48 f3 c6 89 9b 06 |..H.....|
00000038

The protocol buﬀer is the last 24 bytes. This buﬀer decodes into two fields: a `key_id` (16 byte value `(04 14 24 34 44 54 64 74 84 94 a4 b4 c4 d4 e4 f4)`, and a `protection_scheme` (a `var-int` that decodes to `63 62 63 73` or `‘cbcs’`). While this example contains only two fields, additional optional fields could be present.

### PlayReady

Here is unpacked form of the PlayReady base64 string (a PlayReady Object).

00000000 be 01 00 00 01 00 01 00 b4 01 3c 00 57 00 52 00 |..........<.W.R.|
00000010 4d 00 48 00 45 00 41 00 44 00 45 00 52 00 20 00 |M.H.E.A.D.E.R. .|
00000020 78 00 6d 00 6c 00 6e 00 73 00 3d 00 22 00 68 00 |x.m.l.n.s.=.".h.|
00000030 74 00 74 00 70 00 3a 00 2f 00 2f 00 73 00 63 00 |t.t.p.:././.s.c.|
00000040 68 00 65 00 6d 00 61 00 73 00 2e 00 6d 00 69 00 |h.e.m.a.s...m.i.|
00000050 63 00 72 00 6f 00 73 00 6f 00 66 00 74 00 2e 00 |c.r.o.s.o.f.t...|
00000060 63 00 6f 00 6d 00 2f 00 44 00 52 00 4d 00 2f 00 |c.o.m./.D.R.M./.|
00000070 32 00 30 00 30 00 37 00 2f 00 30 00 33 00 2f 00 |2.0.0.7./.0.3./.|
00000080 50 00 6c 00 61 00 79 00 52 00 65 00 61 00 64 00 |P.l.a.y.R.e.a.d.|
00000090 79 00 48 00 65 00 61 00 64 00 65 00 72 00 22 00 |y.H.e.a.d.e.r.".|
000000a0 20 00 76 00 65 00 72 00 73 00 69 00 6f 00 6e 00 | .v.e.r.s.i.o.n.|
000000b0 3d 00 22 00 34 00 2e 00 33 00 2e 00 30 00 2e 00 |=.".4...3...0...|

00000100 20 00 41 00 4c 00 47 00 49 00 44 00 3d 00 22 00 | .A.L.G.I.D.=.".|
00000110 41 00 45 00 53 00 43 00 42 00 43 00 22 00 20 00 |A.E.S.C.B.C.". .|
00000120 56 00 41 00 4c 00 55 00 45 00 3d 00 22 00 4e 00 |V.A.L.U.E.=.".N.|
00000130 43 00 51 00 55 00 42 00 46 00 52 00 45 00 64 00 |C.Q.U.B.F.R.E.d.|
00000140 47 00 53 00 45 00 6c 00 4b 00 53 00 30 00 78 00 |G.S.E.l.K.S.0.x.|
00000150 4e 00 54 00 6b 00 39 00 41 00 3d 00 3d 00 22 00 |N.T.k.9.A.=.=.".|

00000180 50 00 52 00 4f 00 54 00 45 00 43 00 54 00 49 00 |P.R.O.T.E.C.T.I.|

000001be

The PlayReady Header is the string below. (Converted from UTF-16 with indentation and line breaks added for clarity.)

The `ALGID` attribute indicates the protection scheme is ‘cbcs’.

Here is the unpacked form of the `KID` element’s `VALUE` attribute, which is a base64 encoded string.

00000000 34 24 14 04 54 44 74 64 84 94 a4 b4 c4 d4 e4 f4 |4$..TDtd........|
00000010

This is a UUID in Microsoft’s GUID form. That is, three little-endian numbers (4 bytes, 2 bytes, 2 bytes) and an eight-byte sequence. In this example the same key identifier is used for PlayReady and Widevine.

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/about-the-common-media-application-format-with-http-live-streaming-hls

- HTTP Live Streaming
- About the Common Media Application Format with HTTP Live Streaming (HLS)

Article

# About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

## Overview

The Common Media Application Format (CMAF) for segmented media is an extensible standard for the encoding and packaging of segmented media objects for delivery and decoding on end user devices in adaptive multimedia presentations. Delivery and presentation are abstracted by a hypothetical application model that allows a wide range of implementations including HLS and MPEG’s Dynamic Adaptive Streaming over HTTP (MPEG DASH). The CMAF specification defines several logical media objects:

**CMAF Track:** Tracks contain encoded media samples, including audio, video, and subtitles. Media samples are stored in a CMAF specified container derived from the ISO Base Media File Format. Media samples may optionally be protected by MPEG Common Encryption. Tracks are made up of a CMAF Header and one or more CMAF Fragments.

**CMAF Switching Set:** Switching sets contain alternative tracks that can be switched and spliced at CMAF Fragment boundaries to adaptively stream the same content at different bit rates and resolutions.

**Aligned CMAF Switching Set:** Two or more CMAF Switching Sets encoded from the same source with alternative encodings, for example, different codecs, and time aligned to each other.

**CMAF Selection Set:** A group of switching sets of the same media type that may include alternative content (for example, different languages or camera angles) or alternative encodings (for example, different codecs).

**CMAF Presentation:** One or more presentation time synchronized selection sets.

The CMAF Hypothetical Reference Model defines how tracks can be delivered, combined, and synchronized in CMAF Presentations, but the model allows the use of any compatible implementation. It’s possible to create HLS Playlists and a DASH Media Presentation Description that share the same resources, CMAF Addressable Objects, thereby allowing efficient caching even when delivering to multiple platforms. CMAF Addressable Media objects consist of:

**CMAF Header:** Headers contain information that includes information for initializing a track.

**CMAF Segment:** A sequence of one or more consecutive fragments from the same track.

**CMAF Chunk:** A chunk contains a sequential subset of samples from a fragment.

**CMAF Track File:** A complete track in one ISO\_BMFF file.

### Support for CMAF

Apple’s HLS specification is a published RFC, RFC 8216. However, HLS continues to evolve, so there’s an updated draft specification — draft-pantos-hls-rfc8216bis.

The HLS specification defined support for fragmented MPEG-4 Segments (ISO\_BMFF) in September 2016. Clients based on earlier revisions will likely not be able to handle CMAF content. Apple hardware running iOS 10.0, macOS 10.12, and tvOS 10.0 or later OS versions should support CMAF content.

### Manifests, resources, and CMAF presentations

In HLS, the role of the Manifest is divided between the HLS Multivariant Playlist and the Media Playlists it references. They describe a single CMAF Presentation or a sequence of CMAF Presentations.

In an HLS Multivariant Playlist, `EXT-X-STREAM-INF` tags define different tiers of the presentation. Tiers are distinguished by bit rate, required codecs, resolution, and other attributes. Each tier specifies an HLS Media Playlist. Each tier may also indicate additional HLS Renditions, which are Media Playlists described in `EXT-X-MEDIA` tags that are available for selection while playing that tier. For example, an audio Rendition can be used to supply audio if the tier’s Media Playlist only contains video; a group of audio Renditions can be used to offer a selection of different language tracks.

Because CMAF Segments can’t, in general, contain multiple media types, `EXT-X-MEDIA` tags need to be used to associate audio and subtitle Playlists with video, which is usually in the `EXT-X-STREAM-INF` tag’s Media Playlist. The same Rendition can be used by several `EXT-X-STREAM-INF` tags; for instance, multiple video tiers can specify the same audio Rendition. Alternately, higher bit rate video tiers can specify separate, higher bit rate audio Renditions so that audio quality scales with video quality.

### CMAF Tracks, Segments, Headers, and Fragments

There should be one HLS Media Playlist per CMAF Track. In HLS Media Playlists, CMAF Segments are used as HLS Segments. There has to be an `EXT-X-MAP` tag applied to each HLS Segment; the tag points to a CMAF Header that’s appropriate for all CMAF Fragments inside the HLS Segment. Since all CMAF Fragments are independently decodable, their HLS Playlists should contain an `EXT-X-INDEPENDENT-SEGMENTS` tag. When the media is encrypted, EXT-X-SESSION-KEY tags should be included in the Multivariant Playlist to enable prefetching of keys.

The `EXT-X-BYTERANGE` tag can be used to indicate that an HLS Segment is a byte range inside a larger resource.

Media Segments inside `EXT-X-I-FRAMES-ONLY` Playlists start on a CMAF Fragment boundary.

The ` EXT-X-DISCONTINUITY` tag can be used to concatenate multiple CMAF Tracks of the same media type in a Media Playlist. Each discontinuity demarcates a boundary between successive CMAF Presentations. A discontinuity allows the resetting of presentation timestamps and other characteristics. Many changes can require a discontinuity, for example, switching from Sample Encryption to unencrypted. A new `EXT-X-MAP` tag is usually required after a discontinuity. For further information, see the HLS specification.

HLS supports all CMAF subtitle and caption formats, except for IMSC1 Image Tracks.

You can include one or more Event Message boxes ( `‘emsg’`) in each segment. You must use version 1 of the Event Message box standard found in ISO-23009-1. The following values define the semantics:

`scheme_id_uri`

Set to `https://aomedia.org/emsg/ID3` to identify boxes that carry ID3v2 metadata.

`value`

The URI that defines the semantics of the ID field. Any relative URI is considered to be relative to `scheme_id_uri`.

`message_data`

Contains data compatible with ID3 version 2.x.x.

### CMAF Switching Sets

Each Track in a video CMAF Switching Set should appear in the Multivariant Playlist as a Media Playlist URI prefixed by an `EXT-X-STREAM-INF` tag describing it. The `EXT-X-STREAM-INF` tag should also specify any other renditions, such as audio that are intended to play with the video by indicating an appropriate `EXT-X-MEDIA GROUP-ID`.

Each Track in an audio CMAF Switching Set should be represented in the Multivariant Playlist by an `EXT-X-MEDIA` tag. The URI attribute of the `EXT-X-MEDIA` tag should be a URI to that Track’s Media Playlist. It has to have a `GROUP-ID` attribute that allows it to be associated with one or more `EXT-X-STREAM-INF` tags, which specify video tiers.

### CMAF Selection Sets

In HLS, when multiple codecs are offered, `EXT-X-STREAM-INF` tags in the Multivariant Playlist are typically arranged in sets of parallel tiers, for example, `low-bitrate-codec-A`, ` high-bitrate-codec-A`, `low-bitrate-codec-B`, `high-bitrate-codec-B`.

CMAF Selection Sets generally offer either alternate encodings of the same source content (for example, encoded with different codecs) or homogenous encodings of different versions of the source content (for example, different audio language tracks).

For Selection Sets offering codec variants, each Switching Set in the Selection Set should appear as a set of `EXT-X-STREAM-INF` tags, for video, or a set of `EXT-X-MEDIA` tags, for other media types. See CMAF Switching Sets.

For Selection Sets offering source variants, each Track of a member Switching Set should appear as an `EXT-X-MEDIA` tag. Tracks encoded with the same settings should get the same `EXT-X-MEDIA GROUP-ID`. For example, a Selection Set containing French and English Switching Sets, with just one Track in each Switching Set, should appear as two `EXT-X-MEDIA` tags with the same `GROUP-ID`. For more `EXT_X_MEDIA` tag rules, see RFC 8216 and HTTP Live Streaming 2nd Edition.

### CMAF Presentation Profiles

The CMAF specification defines three presentation profiles: unencrypted, encrypted with `‘cbcs’`, and encrypted with `‘cenc’`. HLS supports unencrypted and encrypted with `‘cbcs’`.

### HLS example

In this example, there’s a video CMAF Track containing 29.97 fps video in 60-frame GOPs, each 2.002 seconds long. Each GOP forms a CMAF Fragment. The CMAF Fragments, V1, V2, V3, V4, and V5, total 10.010 seconds of video. Their CMAF Header is `VH`.

Accompanying the video is an English audio CMAF Track consisting of an English CMAF Header, `EH`, and five audio CMAF Fragments: E1, E2, E3, E4, and E5, encoded at a sample rate of 44.1 Khz. Each CMAF Segment is 86 AAC frames, with a duration of 1.997 seconds each, except for E5, which has 87 frames, for a total of 10.008 seconds of audio. There are also five French audio CMAF Fragments — F1, F2, F3, F4, and F5 — and a French CMAF Header, `FH`.

The CMAF Fragments have been packaged into three CMAF Segments per track for delivery and those CMAF Resources identified as HLS segments: `V1andV` 2, `V3andV4`, and `V5`; `E1andE2`, `E3andE4`, and `E5`; and so on.

In addition, there’s a high quality video Track containing CMAF Fragments: `VHQ1`, `VHQ2`, `VHQ3`, `VHQ4`, and `VHQ5`, with Header `VHQH`, packaged and identified similarly.

The two video Tracks, V and VHQ, are CMAF Switching Sets. Each audio Track can also be considered a Switching Set, with only one member. Together, both audio Switching Sets form a CMAF Selection Set.

**Media Playlists**

The HLS Media Playlist for the regular video Track `video.m3u8` would be as follows.

#EXTINF:4.004,
V1andV2
#EXTINF:4.004,
V3andV4
#EXTINF:2.002,
V5
#EXT-X-ENDLIST

The Media Playlist for the high quality video Track `video-hq.m3u8` would be similar.

The Media Playlist for the English audio Track `english.m3u8` would be as follows.

#EXTINF:3.9938,
E1andE2
#EXTINF:3.9938,
E3andE4
#EXTINF:2.0201,
E5
#EXT-X-ENDLIST

The Media Playlist the French audio Track `french.m3u8` would be similar.

**Basic Multivariant Playlist**

The HLS Multivariant Playlist might look like the following example.

#EXT-X-STREAM-INF:BANDWIDTH=1123000,CODECS="avc1.64001f,mp4a.40.2",AUDIO="audio-stereo-64",RESOLUTION=620x334
video.m3u8

#EXT-X-STREAM-INF:BANDWIDTH=8123000,CODECS="avc1.640028,mp4a.40.2",AUDIO="audio-stereo-64",RESOLUTION=1916x1032
video-hq.m3u8

**Multivariant Playlist with Codec Variants**

We could also supply HEVC versions of `video.m3u8` and `video-hq.m3u8`, and perhaps give the high-bandwidth tier better-quality audio. Then the Multivariant Playlist might look like the following example.

#EXT-X-STREAM-INF:BANDWIDTH=1123000,CODECS="avc1.64001f,mp4a.40.2",AUDIO="audio-stereo-64",RESOLUTION=620x334

#EXT-X-STREAM-INF:BANDWIDTH=8187000,CODECS="avc1.640028,mp4a.40.2",AUDIO="audio-stereo-128",RESOLUTION=1916x1032

#EXT-X-STREAM-INF:BANDWIDTH=623000, CODECS="hvc1.1.6.L120.B0,mp4a.40.2",AUDIO="audio-stereo-64",RESOLUTION=620x334
hevc-video.m3u8

#EXT-X-STREAM-INF:BANDWIDTH=4187000, CODECS="hvc1.1.6.L120.B0,mp4a.40.2",AUDIO="audio-stereo-128",RESOLUTION=1916x1032
hevc-video-hq.m3u8

This example illustrates how CMAF Selection Sets can appear as separate Renditions, `english.m3u8` and `french.m3u8`, or as separate sets of tiers distinguished by different required codecs: `{video.m3u8, video-hq.m3u8}` is the AVC Switching Set; `{hevc-video.m3u8, hevc-video-hq.m3u8`} is the HEVC Switching Set. Together they form a Selection Set that allows selection by codec.

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/enabling-low-latency-http-live-streaming-hls

- HTTP Live Streaming
- Enabling Low-Latency HTTP Live Streaming (HLS)

Article

# Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

## Overview

The HLS protocol delivers live and on-demand content streams to global-scale audiences. Historically, HLS has favored stream reliability over latency. Low-Latency HLS extends the protocol to enable low-latency video streaming while maintaining scalability. The new low-latency mode lowers video latencies over public networks into the range of standard television broadcasts.

Backend production tools and content delivery systems must implement new rules to enable low-latency stream playback. Low-Latency HLS offers new functionality in these areas:

- Generation of partial segments

- Playlist delta updates

- Blocking of playlist reload

- Using preload hints

- Rendition reports

The HLS specification defines low-latency extensions in HTTP Live Streaming 2nd Edition revision 7 and later.

### Generate Partial Media Segments

Low-Latency HLS provides a parallel channel for distributing media at the live edge of the Media Playlist, which divides the media into a larger number of smaller files, such as CMAF Chunks. These smaller files are called HLS Partial Segments. Because each Partial Segment has a short duration, it can be packaged, published, and added to the Media Playlist much earlier than its Parent Segment.

While regular Media Segments might be 6 seconds each, an example Partial Segment might be only 200 milliseconds. A first Partial Segment might publish only 200 milliseconds after the previous segment publishes, followed by 29 of its peers, followed at last by a regular-length, 6-second Media Segment containing the same media as the concatenation of its 30 Partial Segments. In order to reduce Playlist bloat, the server removes Partial Segments from the Media Playlist once they’re greater (older) than three target durations from the live edge.

You add Partial Segments to the Media Playlist using the new `EXT-X-PART` tag. You can place other Media Segment Tags (such as `EXT-X-DISCONTINUITY`) at Parent Segment boundaries.

A Partial Segment must be in one of the Supported Media Segment Formats described in section 3.1 of HTTP Live Streaming 2nd Edition.

### Provide Playlist Delta Updates

Clients transfer playlists more frequently with Low-Latency HLS. They can request and servers can provide Playlist Delta Updates, which reduce this transfer cost. These updates replace a considerable portion of the Playlist that the client already has with the new `EXT-X-SKIP` tag.

### Blocking Playlist reloads

To support efficient client notification of new Media Segments and Partial Segments, Low-Latency HLS introduces the ability to block a Playlist reload request. When a client issues an HTTP GET to request a Media Playlist update, it can add special query parameters called Delivery Directives to specify that it wants the Playlist response to include a future segment. The server then holds onto the request (blocks) until a version of the Playlist that contains that segment is available. Blocking Playlist Reloads eliminates Playlist polling.

### Provide Preload Hints and Blocking of Media Downloads

Eliminating unnecessary round trips is critical when delivering low-latency streams at global scale. Servers use a new tag, `EXT-X-PRELOAD-HINT`, to inform clients of upcoming Partial Segments and Media Initialization Sections. A client can issue a GET request for a hinted resource in advance; the server responds to the request as soon as the media becomes available.

### Provide Rendition Reports

When playing at low latency, the client must be able to switch renditions with a minimum number of round trips in order to perform bit-rate adaptation. To support this, the server adds Rendition Reports on the other renditions in the Multivariant Playlist to each Media Playlist. The `EXT-X-RENDITION-REPORT` tag carries a Rendition Report and provides information, such as the last Media Sequence Number and Part currently in the Media Playlist of that rendition.

### Add Low-Latency HLS Delivery Directives

HLS now defines Delivery Directives, which are special query parameters that can be added to the URL of a GET request for a Playlist. These Delivery Directives include:

Indicates that the server must hold the request until a Playlist contains a Media Segment with Media Sequence Number of M or later.

Indicates, in combination with `_HLS_msn`, that the server must hold the request until a Playlist contains Partial Segment N of Media Sequence Number M or later. The first Partial Segment of a segment is `_HLS_part=0`, the second is `_HLS_part=1`, and so on. The `_HLS_part` parameter requires an `_HLS_msn` parameter.

`_HLS_skip=YES|v2`

Requests a Playlist Delta Update, in which the earlier portion of the Playlist is replaced with an `EXT-X-SKIP` tag.

### Utilize New Media Playlist Tags for Low-Latency HLS

The following Playlist tags support Low-Latency HLS.

`EXT-X-SERVER-CONTROL`

Allows the server to indicate support for features such as Blocking Playlist Reload and Playlist Delta Updates.

`EXT-X-PART-INF`

Provides information about HLS Partial Segments in the Playlist.

`EXT-X-PART`

Identifies a Partial Segment in the Playlist.

`EXT-X-PRELOAD-HINT`

Hints that a resource or a byte range of a resource are needed to play back an upcoming part of the presentation.

Note that when a hinted Partial Segment eventually appears in the Playlist as an `EXT-X-PART` tag, it may be different than previous Partial Segment. It may have a different Discontinuity Sequence Number, Media Initialization Section, or encryption configuration. In other words, the Partial Segment can be preceded by an `EXTINF` tag indicating the end of the previous Parent Segment and an `EXT-X-DISCONTINUITY`, `EXT-X-MAP`, or `EXT-X-KEY` tag.

A server may choose not to publish a previously hinted Partial Segment if the planned segmentation changes, such as in the case of early return from an ad.

`EXT-X-RENDITION-REPORT`

Carries information about an associated rendition that’s as up to date as the Playlist that contains it.

`EXT-X-SKIP`

When a server issues a Playlist Delta Update, it replaces Media Segments earlier than the Skip Boundary and their associated tags with an ` EXT-X-SKIP` tag.

### Comply with the Low-Latency Server Configuration Profile

To support timely delivery of media, Low-Latency HLS requires certain transport features beyond what is necessary for regular HLS. These requirements are defined in the Low-Latency Server Configuration Profile. Because the Low-Latency HLS syntax is backward-compatible with existing HLS, clients fall defines the Low-Latency Server Configuration Profile in Appendix B.

### Expect Delivery from CDN Tune-In

Players of Low-Latency HLS should expect delivery of low-latency streams through CDNs and other HTTP caches. To start playback at low latency, the client must first obtain a reasonably up-to-date version of the Media Playlist. Appendix C of HTTP Live Streaming 2nd Edition describes an efficient approach for obtaining an up-to-date Media Playlist served through an HTTP cache.

### Examine a Low-Latency HLS Playlist

Here’s an example of a low-latency playlist. As mentioned above, the Low-Latency HLS syntax is backward-compatible, so we can use a version number of six. Clients that do not understand the Low-Latency tags will ignore them.

#EXTINF:4.00008,
fileSequence264.mp4
#EXTINF:4.00008,
fileSequence265.mp4
#EXTINF:4.00008,
fileSequence266.mp4
#EXTINF:4.00008,
fileSequence267.mp4
#EXTINF:4.00008,
fileSequence268.mp4
#EXTINF:4.00008,
fileSequence269.mp4
#EXTINF:4.00008,
fileSequence270.mp4
#EXTINF:4.00008,
fileSequence271.mp4
#EXTINF:4.00008,
fileSequence272.mp4

#EXT-X-RENDITION-REPORT:URI="../4M/waitForMSN.php",LAST-MSN=273,LAST-PART=1

### Examine a Playlist Delta Update

Here’s an example of a playlist delta update. Note that use of tha EXT-X-SKIP tag requires a later version than the basic use of Low-Latency HLS above.

#EXTINF:4.00008,
#EXTINF:4.00008,
fileSequence267.mp4
fileSequence268.mp4
#EXTINF:4.00008,
#EXTINF:4.00008,
fileSequence269.mp4
fileSequence270.mp4
#EXTINF:4.00008,
#EXTINF:4.00008,
fileSequence271.mp4
fileSequence272.mp4

#EXT-X-RENDITION-REPORT:URI="../4M/waitForMSN.php",LAST-MSN=273,LAST-PART=3

### Examine Byterange-Addressed Parts

Here’s an example of a byterange-addressed part. In a real playlist at least some of the EXT-X-PART tags would contain an INDEPENDENT attribute. Those have been removed to make the example clearer.

#EXTINF:4.08,
fs270.mp4

#EXTINF:4.08,
#EXTINF:4.08,
fs270.mp4
fs271.mp4

#EXTINF:4.08,
#EXTINF:4.08,
#EXT-X-PRELOAD-HINT:TYPE=PART,URI="fs272.mp4",BYTERANGE-START=21000

### Revision History

The following table describes the changes to the Protocol Extension for Low-Latency HLS.

| Date | Notes |
| --- | --- |
| 2024-05-21 | Added some clarifying text. |
| 2024-01-16 | Corrected errors in examples. |
| 2021-11-12 | Renamed “primary playlist” to “Multivariant Playlist.” |
| 2021-01-11 | Added missing double quotes around `BYTERANGE` parameters. |
| 2020-05-04 | Moved protocol rules to the HLS spec. This document is now a descriptive supplement. |
| 2020-02-05 | Added additional information related to preload hints and blocking of media downloads. |
| 2019-08-22 | Removed the `_HLS_report` parameter and made Rendition Reports mandatory. Clarified the `LAST-MSN` definition. |
| 2019-07-25 | Added the CDN Tune-in appendix. |
| 2019-07-10 | Updated MSN and part validation rules. Made server response recommended instead of mandatory. Added the requirement of the AGE header when using HTTP proxy caches. |
| 2019-06-03 | Added a new document describing Low-Latency HLS. |

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/links-to-additional-specifications-and-videos

- HTTP Live Streaming
- Links to additional specifications and videos

Article

# Links to additional specifications and videos

Review additional specifications and documents.

## Overview

The following links are in addition to the specifications listed below.

- RFC 8216. The IETF Informational specfication for HTTP Live Streaming. This document describes the HTTP Live Streaming protocol as of August 2017. This document specifies the data format of the files and the actions to be taken by the server and the clients of the streams.

- FairPlay Streaming. A technology describing how to secure the delivery of streaming media to devices through the HTTP Live Streaming protocol. Using FairPlay Streaming (FPS) technology, content providers, encoding vendors, and delivery networks can encrypt content, securely exchange keys, and protect playback on iOS, tvOS, and Safari on macOS.

- MPEG-2 Stream Encryption Format for HTTP Live Streaming. This document describes a sample-level encryption format for several types of elementary streams that can be carried in MPEG-2 transport streams ISO/IEC 13818-1 and MPEG elementary audio streams.

- Timed Metadata for HTTP Live Streaming. This document describes how ID3 metadata is carried as timed metadata in MPEG-2 Transport Streams as used by the HTTP Live Streaming protocol.

- Providing JavaScript Object Notation (JSON) chapters. This document describes how to provide chapter markers and other per-chapter metadata used by iOS, tvOS, and macOS for HTTP Live Streaming (HLS).

- Carriage of ID3 Timed Metadata in the Common Media Application Format (CMAF). This document defines how ID3 metadata are carried as timed metadata in Common Media Application Format (CMAF) compatible fragmented MP4 streams using Event Message boxes.

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/videos-about-hls

- HTTP Live Streaming
- Videos about HLS

Article

# Videos about HLS

Review informational videos about HTTP Live Streaming.

## Overview

The following WWDC videos provide additional information about HTTP Live Streaming.

- Preparing and Presenting Media for Accessibility: AVFoundation automatically selects appropriate audio and subtitle tracks in your media. Learn how media selection works and find out how to author media with accessibility features like subtitles and closed captions. Go beyond the basics to use AVFoundation for customizing subtitle appearance and presentation.

- Content Protection for HTTP Live Streaming: FairPlay streaming provides industrial-grade protection for audio and video content. Learn how to implement and deploy FairPlay streaming to protect content when using HTTP Live Streaming.

- Validating HTTP Live Streams: HTTP Live Streaming enables the reliable delivery of media content over a wide variety of network conditions. Learn best practices in HLS authoring, see how to verify your streams using the HTTP Live Streaming tools, and apply the results to improve the performance of your streams.

- What’s New in HTTP Live Streaming: HTTP Live Streaming offers a reliable media playback experiences over a wide variety of network conditions. Join us to learn how to deliver offline playback using the same media assets you already host for online playback. See new additions to the HLS protocol, such as support for fragmented MP4 and in-playlist metadata.

- HLS Authoring Update: HTTP Live Streaming (HLS) reliably delivers video to audiences around the world. Key to this reliability is a comprehensive set of tools to help you author, deliver, and validate the HLS streams you create. See what’s new in these tools, learn the latest authoring recommendations, and how they apply to advances in HLS such as support for HEVC and IMSC1.

- Error Handling Best Practices for HTTP Live Streaming: HTTP Live Streaming (HLS) reliably delivers media content across a variety of network and bandwidth conditions. However, there are many factors that can impact stream delivery, such as server or encoder failures, caching issues, or network dropouts. Learn the best-practice behaviors that your servers should adopt to maximize reliability, and gain a practical understanding of the errors your app may encounter and how to handle them.

- Advances in HTTP Live Streaming: HTTP Live Streaming allows you to stream live and on-demand content to global audiences. Learn about great new features and enhancements to HTTP Live Streaming. Highlights include support for HEVC, playlist metavariables, IMSC1 subtitles, and synchronized playback of multiple streams. Discover how to simplify your FairPlay key handling with the new AVContentKeySession API, and take advantage of enhancements to offline HLS playback.

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/providing-metadata-for-xhe-aac-video-soundtracks

- HTTP Live Streaming
- Providing metadata for xHE-AAC video soundtracks

Article

# Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

## Overview

Soundtracks that use xHE-AAC (Extended High-Efficiency Advanced Audio Codec) encoding include MPEG-D DRC metadata for loudness and dynamic range control (DRC). When you create video soundtracks with xHE-AAC, provide at least the following metadata to ensure consistent results across different services. For playback, set up the MPEG-D DRC tool at the decoder by following the guidelines below.

### Configure metadata for content generation

The loudness and DRC metadata that you include in video content needs to fulfill the MPEG-D DRC requirements for the Basic DRC Metadata Profile, and always include the following values:

**Loudness Metadata**

| loudness info fields | value |
| --- | --- |
| Include a `methodValue` for `methodDefinition` == “Anchor Loudness” and `measurementSystem` == “ITU-R BS.1770” | Measure anchor loudness using speech-gating or estimate when speech activity is low. |
| `bs_true_peak_level` or `bs_sample_peak_level` | True peak according to ITU-R BS.1770 or sample peak level. |

Measure anchor loudness of the dialog stem using the ITU-R BS.1770 standard because `methodValue` must reflect the actual anchor loudness of the content. Apply speech-gating to the full mix to obtain the anchor loudness value when only the full mix is available for measurement.

Anchor loudness can be inaccurate when the speech detector can’t find much speech in the full mix. Monitor this situation by computing the speech activity, which is the duration of detected speech divided by the duration of the content. When speech activity is low, ignore this measurement because it can be inaccurate. Instead, derive the anchor loudness value from the program loudness value and other applicable measurements to model the value from statistics of a variety of content. See Adjusting anchor loudness for additional information.

**DRC Metadata**

| `drcSetEffect` of the required DRC metadata | Required minimum level that supports playback with minimal peak limiter engagement (LKFS) | Position of bit in `drcSetEffect` field of `drcInstructions`, which must have a value of `1` |
| --- | --- | --- |
| `Late Night` | -24 | 1 |
| `Noisy Environment` | -16 | 2 |
| `Limited Playback Range` | -16 | 3 |
| `General Compression` | -24 | 6 |

Match as close as possible the output anchor loudness of the DRC-processed versions with the anchor loudness of the unprocessed output.

The DRC for `General Compression` can have several instances to accommodate various target loudness values, which provides just enough compression to reach the target without engaging a limiter. If no compression is necessary or desired for specific loudness targets, include a corresponding DRC for `General Compression` that doesn’t have a compression effect.

### Configure metadata for playback

Configure the MPEG-D DRC decoder for playback according to the specifications below. The configuration occurs completely or partially at the system level and those settings don’t appear at the API level.

Set up the MPEG-D DRC decoder to assign the highest priority to the following loudness metadata:\*\*\*\*

| Metadata field | Value (highest priority) |
| --- | --- |
| `methodDefinition` | `Anchor Loudness` |
| `measurementSystem` | `Expert/Panel` |

The `methodDefinition` field defaults to `Program Loudness`, if present, if you don’t specify `Anchor Loudness`. This configuration deviates from the default configuration specified in ISO/IEC 23003-4, which selects `Program Loudness` and `ITU-R BS.1770` with highest priority. However, the standard specifies an interface to customize the configuration, including the loudness metadata priority.

Some previously deployed implementations may use the default ISO/IEC 23003-4 configuration and may not support the interface for customization. These systems may select loudness metadata with a `methodDefinition` value of `Program Loudness`, if present, in addition to other loudness metadata. This can result in a deviation of the output loudness of the same content from systems that select `Anchor Loudness`, if present, in addition to `Program Loudness`.

The following table (ANSI/CTA-2075) provides recommended target loudness value settings of the DRC tool to control the integrated loudness at the output:

| Transducer SPL range | Maximum SPL (dBA) | Target loudness (LKFS) |
| --- | --- | --- |
| `small` | below 75 | -16 |
| `medium` | between 70 and 90 | -24 |
| `large` | above 85 | -31 |
| `unknown` | NA | -24 |

To achieve sufficient output SPL, ensure the target loudness value depends on the SPL range of the active transducer, which has three categories ( `small`, `medium`, `large`). Choose the SPL range category by measuring the maximum SPL of the transducer at the anticipated listener location using pink noise at -24 LKFS. Assign the category according to the middle column as ANSI/CTA-2075 Annex G describes. For example, micro loudspeakers in portable devices typically fall into the `small` SPL range category.

The following table specifies the appropriate DRC requests for different listening environments and transducer SPL ranges (ANSI/CTA-2075):

| Environment | Transducer SPL range | DRC request |
| --- | --- | --- |
| `ideal`, `unknown` | small | `limited` |
| `ideal`, `unknown` | `large`, `medium`, `unknown` | `general` |
| `noisy` | all | `noisy` |

Request `general` for DRC when you want loudness normalization unless a different DRC request is applicable for the playback scenario. This applies appropriate compression to reach the target loudness, such as when applying gain during normalization.

User preferences can override DRC settings. The following table provides examples of two preferences and the conditions, transducer SPL range, and environment under which to apply these preferences:

| User preference | Environment | Transducer SPL range | DRC request |
| --- | --- | --- | --- |
| `max DRC` | all | all | `noisy` |
| `late night` | `ideal`, `unknown` | `large`, `medium`, `unknown` | `late night` |

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/adjusting-anchor-loudness

- HTTP Live Streaming
- Adjusting anchor loudness

Article

# Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

## Overview

Apply the adjustment method below to improve the consistency of your anchor loudness, or standard, value for low speech activity. The method’s basis is a statistical model of anchor loudness for a large variety of long-form content that takes advantage of the correlation with other loudness-based measurements. The method uses the following measurements:

- Speech-gated loudness

- Speech activity that derives from a speech detector

- Program loudness (ITU-R BS.1770-4)

- Top value of LRA (loudness range) (EBU Tech 3342)

For low speech activity, the model ignores the speech-gated loudness value and computes anchor loudness from the other three measurements. A gradual transition from the model to the measured, speech-gated loudness occurs as the speech activity increases.

The following examples and source code show how to calculate anchor loudness using program loudness and speech-gated loudness.

### Determine anchor loudness using different program loudness values

The following figure shows a visual representation of anchor loudness for an example with a speech-gated loudness of -27 LKFS (loudness, K-weighted, relative to full scale) and different program loudness values.

The lines on the left correspond to the calculated anchor loudness as a result of the adjustment method. The labels for each line indicate the program loudness values. For low speech activity, anchor loudness increases with program loudness. For increasing speech activity, there’s a transition to the speech-gated loudness measurement.

The next figure displays anchor loudness for an example with speech-gated loudness of -27 LKFS and program loudness of -24 LKFS. The difference between top value of LRA and program loudness characterizes how dynamic the content is. The lines on the left correspond to the calculated anchor loudness as a result of the adjustment method. The labels for each line indicate the value of the loudness difference in loudness units (LU). The loudness difference correlates with anchor loudness, and the modeling results in lower anchor loudness for more dynamic content at low speech activity. As the speech activity increases, anchor loudness transitions to the measured speech-gated loudness.

The following source code includes a function to compute the adjusted anchor loudness value from the parameters in the preceding examples, which is applicable to long-form content.

enum AnchorLoudnessAdjustmentError: Error {
case speechActivityOutOfBounds
}

/// Computes adjusted anchor loudness
/// - Parameters:
/// - programLoudness: The loudness (LKFS) produced by ITU-R BS.1770-4.
/// - speechLoudness: The loudness (LKFS) produced by ITU-R BS.1770-4 applied to the speech-gated content.
/// - activity: The ratio of speech-gated content duration and content duration.
/// - isLraTopPresent: If `true`, the top value of LRA measurement is available.
/// - lraTop: The loudness (LKFS) produced by taking the top value of loudness range according to EBU Tech 3342.
/// - Returns: Adjusted anchor loudness (LKFS)
func adjustedAnchorLoudnessFor(programLoudness: Double,
speechLoudness: Double,
activity: Double,
isLraTopPresent: Bool,

guard (0...1).contains(activity) else {
throw AnchorLoudnessAdjustmentError.speechActivityOutOfBounds
}

// Constants
/// Ignore `speechLoudness` below this speech activity ratio.
let activityLow = 0.17
/// Keep `speechloudness` above this speech activity ratio.
let activityHigh = 0.25
/// The boundary for the difference of `anchorLoudness` and `programLoudness`.`
let loudnessOffsetDefault = 3.0
/// The upper limit for the difference of `programLoudness` and `anchorLoudness`.
let loudnessOffsetMax = 8.0
/// The lower limit for the difference of `programLoudness` and `anchorLoudness`.
let loudnessOffsetMin = 0.0
/// The upper limit for the difference of `programLoudness` and `speechLoudness`.
let loudnessDiffMax = 8.0

// Parameters for linear regression models.
let model1ParamA = 6.452208
let model1ParamB1 = 0.301736
let model1ParamB2 = 0.881433
let model2ParamA = 11.549024
let model2ParamB = 0.362253

var loudnessOffset = loudnessOffsetDefault
var speechLoudnessBounded = speechLoudness
var anchorLoudness = speechLoudness

// Limit speech loudness to a reasonable range below program loudness.
let diffLoudness = programLoudness - speechLoudnessBounded

speechLoudnessBounded = programLoudness - loudnessDiffMax
}

speechLoudnessBounded = programLoudness
}

// Compute loudness offset from linear regression model.
if isLraTopPresent {
let plLraTop = max(0, lraTop - programLoudness)
loudnessOffset = model1ParamA +
model1ParamB1 * programLoudness +
model1ParamB2 * plLraTop
} else {
loudnessOffset = model2ParamA + model2ParamB * programLoudness
}

// Clamp `loudnessOffset`.
loudnessOffset = max(loudnessOffsetMin, min(loudnessOffset, loudnessOffsetMax))

// Update anchor loudness according to activity level.

anchorLoudness = speechLoudnessBounded
} else {

let weight = (activity - activityLow) / (activityHigh - activityLow)
anchorLoudness = weight * speechLoudnessBounded +
(1 - weight) * (programLoudness - loudnessOffset)
} else {
anchorLoudness = programLoudness - loudnessOffset
}
}

return anchorLoudness
}

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

---

# https://developer.apple.com/documentation/http-live-streaming/providing-javascript-object-notation-json-chapters

- HTTP Live Streaming
- Providing JavaScript Object Notation (JSON) chapters

Article

# Providing JavaScript Object Notation (JSON) chapters

Prepare JSON chapters for HTTP Live Streaming.

## Overview

Content providers supply chapter markers and other per-chapter meta data using the `EXT-X-SESSION-DATA` tag in the HTTP Live Streaming (HLS) Multivariant Playlist. Apple’s iOS, tvOS, and macOS platforms receive this metadata as JSON, a format that uses human-readable text to define data objects described in RFC 7159.

### Organize chapter metadata

Chapter data is information that describes a chapter using four different types: timing, titles, images, and general metadata. Keep the following in mind when designing your chapter data:

- Each chapter requires a start time and may have an optional duration.

- Each chapter may have multiple titles, images, and metadata items.

- Each title in a chapter has a unique BCP 47 language tag.

- Each metadata item in a chapter has a unique key and language.

Chapter metadata appears as an array of chapters. Each element in the array contains information about that chapter. The first array element describes the first chapter, the second element describes the second chapter, and so on.

Each element in the chapter array is a JSON object called a _chapter entry_. The chapter entry must contain a `start-time`. The chapter entry should contain `titles`, `images`, and possibly `metadata`.

The chapter entry may contain an item named `chapter` to promote human readability of the JSON. It may also contain an item named `duration`. Chapter entries are assumed to have a duration from `start-time` to the `start-time` of the next chapter entry, unless duration is specified. Chapter timing can overlap and nest, in which case both `start-time` and `duration` must be present.

Below is a simple three-chapter example of chapter data formatted as JSON. Only chapter titles and start times are present. Each chapter title is in two different languages: English and Spanish.

[\
{\
"chapter": 1,\
"start-time": 0,\
"titles": [\
{\
"language": "en",\
"title": "birth"\
},\
{\
"language": "es",\
"title": "nacimiento"\
}\
]\
},\
{\
"chapter": 2,\
"start-time": 500.1,\
"titles": [\
{\
"language": "en",\
"title": "life"\
},\
{\
"language": "es",\
"title": "vida"\
}\
]\
},\
{\
"chapter": 3,\
"start-time": 1200.2,\
"titles": [\
{\
"language": "en",\
"title": "death"\
},\
{\
"language": "es",\
"title": "muerte"\
}\
]\
}\
]

Here’s the general layout of the JSON chapter data format. The JavaScript comments aren’t legal JSON and are for illustrative purposes.

[\
{\
"chapter": number,\
"start-time": number,\
"duration": number,\
"titles": [\
{\
"language": string,\
"title": string\
},\
// … (for each language for this chapter)\
],\
"images": [\
{\
"image-category": string,\
"pixel-width": number,\
"pixel-height": number,\
"url": string\
},\
// … (for each image type for this chapter)\
],\
"metadata": [\
{\
"key": string,\
"value": object | number | string | array,\
"language": string,\
},\
// … for each metadata value for this chapter\
],\
},\
// … for each chapter\
]

### Add titles

Chapter entries may contain a `titles` JSON array. Each element of a `titles` array is a JSON object that must contain both a `language` BCP 47 string and a `title` string with the title for that chapter, written in the language specified by the `language` string. All strings must be encoded using UTF-8. Set the language to `“und”` if the title strings are language-neutral, such as a numeric string.

### Add images

Chapter entries may contain an `images` JSON array. Each element of an `images` array is a JSON object containing information about images for each chapter. For example, an `images` array may contain an element for a thumbnail image and an element for an HD image.

Each element in an `images` array must contain an `image-category` string, a `pixel-width` number, a `pixel-height` number, and a `url` string.

The `image-category` string should be the same across chapters for images that are similar. In the three-chapter case mentioned above, you would use one string for the thumbnails ( `thumbnail`) and a different string for the HD images ( `hd`).

The `url` string must be an absolute or relative URL to the image data associated with the chapter. Relative URLs are relative to the path that contained the JSON chapter document.

The `images` files themselves may be in a variety of image formats. For example, JPEG, PNG, and TIFF are all supported.

### Add metadata

Chapter entries may also contain a metadata JSON array. Each element of a `metadata` array is a JSON object containing metadata for that chapter. Each metadata array element contains a mandatory `key` and `value`, along with an optional `language` BCP-47 string. The key element must be a string. The value element can be a string, number, array, or object. If any `value` is a URI, it’s passed as-is. The system has no way to interpret a relative URI in that context.

### Specify a main playlist

JSON-formatted chapter data must be specified in a main playlist using the `EXT-X-SESSION-DATA` tag for use in HTTP Live Streaming.

The DATA-ID attribute of the `EXT-X-SESSION-DATA` must be `com.apple.hls.chapters`. The URI attribute must point to the JSON-formatted chapter data. The URI may be absolute or relative to the path that contained the main playlist, as shown here:

`#EXT-X-SESSION-DATA:DATA-ID="com.apple.hls.chapters",URI="http://meta.example.com/movie403/chapters.json"`

### Perform validation

Use the following JSON schema to validate your chapter data.

{
"$schema": "http://json-schema.org/draft-04/schema#",
"title": "HLS Chapter Data",
"description": "HLS chapter data format",
"type": "array",
"items": {
"description": "chapter entry",
"type": "object",
"properties": {
"chapter": {
"description": "Chapter number (optional)",
"type": "number",
"minimum": 1
},
"start-time": {
"description": "Chapter start time",
"type": "number",
"minimum": 0
},
"duration": {
"description": "Chapter duration (optional)",
"type": "number",
"minimum": 0,
"exclusiveMinimum": true
},
"titles": {
"description": "List of titles by language for chapter (optional)",
"type": "array",
"items": {
"description": "Title object",
"type": "object",
"properties": {
"language": {
"description": "BCP 47 language code; und for undefined",
"type": "string"
},
"title": {
"description": "Chapter title string",
"type": "string"
}
},
"required": ["language", "title"]
}
},
"images": {
"description": "List of images for chapter (optional)",
"type": "array",
"items": {
"description": "Image object",
"type": "object",
"properties": {
"image-category": {
"description": "Image category",
"type": "string"
},
"pixel-width": {
"description": "Pixel width",
"type": "integer",
"minimum": 0,
"exclusiveMinimum": true
},
"pixel-height": {
"description": "Pixel height",
"type": "integer",
"minimum": 0,
"exclusiveMinimum": true
},
"url": {
"description": "URL to image (relative or absolute)",
"type": "string"
}
},
"required": ["image-category", "pixel-width", "pixel-height", "url"]
}
},
"metadata": {
"description": "List of metadata entries for chapter (optional)",
"type": "array",
"items": {
"description": "Metadata object",
"type": "object",
"properties": {
"key": {
"description": "Key value name",
"type": "string"
},
"value": {
"description": "Metadata value",
"type": ["string", "number", "boolean", "array", "object"]
},
"language": {
"description": "BCP 47 language code (optional)",
"type": "string"
}
},
"required": ["key", "value"]
}
}
},
"required": ["start-time"]
}
}

### Test and access chapter data

`AVAsset` contains details of how to access chapter data. The methods described return an array of `AVTimedMetadataGroup` objects, one object for each chapter. The order of the groups matches the order of the JSON file.

Each `AVTimedMetadataGroup` object has a start time, end time, and a list of `AVMetadataItem`. Every item from the titles, images, and metadata arrays in the JSON is in the list of metadata items.

Images have an `extraAttributes` dictionary. This dictionary contains a key `“iTunesImageResolution”` whose value is a dictionary that contains the `pixel-width`, `pixel-height`, and `image-category` from the JSON entry.

The metadata item keys are placed in the key space `quickTimeMetadata`. This key space defines its key values to be expressed as reverse-DNS strings. This allows you to define your own keys in a well-established way that avoids collisions.

## See Also

### Specifications and other documents

Learn the requirements for live and on-demand audio and video content delivery using HLS.

Using content protection systems with HLS

Adding encryption keys to media playlists

About the Common Media Application Format with HTTP Live Streaming (HLS)

Learn the Common Media Application Format as it applies to HLS.

Enabling Low-Latency HTTP Live Streaming (HLS)

Add Low-Latency HLS to your content streams to maintain scalability.

Links to additional specifications and videos

Review additional specifications and documents.

Videos about HLS

Review informational videos about HTTP Live Streaming.

Providing metadata for xHE-AAC video soundtracks

Ensure volume normalization by including metadata for loudness and dynamic range control.

Adjusting anchor loudness

Adjust anchor loudness when measurements of speech-gated loudness for a full mix may be inaccurate, such as when speech activity is low.

---

# https://developer.apple.com/documentation/http-live-streaming/deploying-a-basic-http-live-streaming-hls-stream)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/preparing-audio-for-http-live-streaming)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/example-playlists-for-http-live-streaming)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/about-the-ext-x-version-tag)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/using-apple-s-http-live-streaming-hls-tools)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/using-content-protection-systems-with-hls)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/about-the-common-media-application-format-with-http-live-streaming-hls)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/enabling-low-latency-http-live-streaming-hls)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/links-to-additional-specifications-and-videos)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/videos-about-hls)



---

# https://developer.apple.com/documentation/http-live-streaming/providing-metadata-for-xhe-aac-video-soundtracks)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/adjusting-anchor-loudness)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/providing-javascript-object-notation-json-chapters)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices).

.#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/providing-javascript-object-notation-json-chapters).

.#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices-appendixes

- HTTP Live Streaming
- HTTP Live Streaming (HLS) authoring specification for Apple devices
- HTTP Live Streaming (HLS) Authoring Specification for Apple devices appendixes

Article

# HTTP Live Streaming (HLS) Authoring Specification for Apple devices appendixes

Learn additional information related to the HLS Authoring Specification for Apple Devices.

## Overview

The appendixes in this article expand on information provided in the HTTP Live Streaming (HLS) authoring specification for Apple devices. It is not intended as a standalone document.

### Testing your streams

Apple provides several command-line tools for HTTP Live Streaming at After signing in with your Apple Developer account, search for _http live streaming tools_.

To assist in validating your streams, use the command-line tools `mediastreamvalidator` and `hlsreport`. While these tools are unable to check everything about your streams, the checks they do are fairly comprehensive and Apple continues to improve the tools.

Check the video quality of your streams by visual inspection. The `mediastreamvalidator` tool does not check video quality, so check playback of your streams under a variety of network conditions.

### Using hlsreport

Use the binary `hlsreport` to generate an HTML summary report from a JSON file that `mediastreamvalidator` creates. The report includes several tables with details about variants, renditions, and I-frame variants. Each table entry has a unique stream ID number. A list of issues is included, divided into Must Fix and Should Fix categories according to this specification. The issues cross-reference individual variants and renditions using the unique stream IDs.

The simplest way to call it is:

`		hlsreport validation_data.json`

where `validation_data.json` is the JSON file that `mediastreamvalidator` generates. This produces a file called `validation_data.html` that is the report. You can change the name of the report file with the `-o` option:

`		hlsreport -o my_report.html validation_data.json`

For further information, see the `hlsreport(1)` man page.

### Declared versus measured values of bandwidths

VOD bit rates are measured over the entirety of the content. Live (linear) bit rates are measured over ~1 hour of content.

| | VOD | Live/Linear |
| --- | --- | --- |
| Measured average bit rate versus AVERAGE-BANDWIDTH (attribute) | within 10% of attribute value | < 110% of attribute value |
| Measured peak bit rate versus BANDWIDTH (attribute) | within 10% of attribute value | < 125% of attribute value |
| Measured peak bit rate versus measured average bit rate | < 200% of measured average | no rule |

### Audio compatibility

Additional information about device and audio format compatibility.

| Devices | AAC (Stereo) | AC-3/E-AC-3 | Dolby Digital Plus with Dolby Atmos |
| --- | --- | --- | --- |
| iOS devices - A12 Bionic based and later | Yes | Yes | Yes |
| Apple TV 4K (1st and 2nd Gen)† | Yes | Yes | Yes |
| OS X devices - 2018 and later | Yes | Yes | Yes |
| iOS and tvOS devices - A7-based or later \*, but not listed above | Yes | Yes | Plays as E-AC-3 |
| Older OS X devices | Yes | Yes | Plays as E-AC-3 |
| Apple TV (3rd Gen), iPhone 5, and iPhone 5C | Yes | Only AC-3 via pass-through | No |
| All older iOS and tvOS devices | Yes | No | No |

See for actual technical specifications.

\*Complete support requires iOS 9.3 or tvOS 9.2, or later. Dolby Digital Plus with Dolby Atmos requires tvOS 12.0 or later.

Dolby Digital Plus with Dolby Atmos† requires tvOS 12.0 or later.

APAC support depends on the capability of the actual device and OS version. See \[APAC\] (https://developer.apple.com/av-foundation/Apple-Positional-Audio-Codec.pdf) specification for support information.

### On bit rates for variants

A number of factors affect the bit rate needed to encode video:

- Codec (for example, H.264 or HEVC)

- Specific encoder implementation and features used

- Resolution (for example, 1920 x 1080, 1280 x 720, and so on)

- Frame rate (for example, 24, 25, 30, 50, 60)

- Bits per pixel (for example, HDR typically uses more bits than SDR)

- Complexity of the content

- Desired subjective quality

These factors make universal encoding recommendations for content difficult. HTTP Live Streaming (HLS) authoring specification for Apple devices includes initial bit rate recommendations that you can evaluate against your content, constraints and encoding workflow.

### I-frame bit rates versus normal bit rates

The formula in item 6.5 (for I-frame bit rates) in HTTP Live Streaming (HLS) authoring specification for Apple devices requires some explanation.

During trick play, the player tries to deliver eight frames per second. If the playback rate implies a higher frame rate, frames will be dropped to keep the frame rate at eight frames per second. If fewer frames are available, it will play at a lower frame rate.

The I-frame bit rate is the bit rate of the rendition if it were played at normal speed. The I-frame rendition may be 2 fps, 1 fps, 0.5 fps, 0.2 fps, or something else. Let F be the frame rate of the I-frame rendition. Then, 8/F is the multiplier, that is, how much the bit rate is increased by playing the rendition at eight frames per second. The bit rate doesn’t increase by more than this factor because the player can’t play more than eight frames per second.

The I-frame rendition should have an effective bit rate similar to the normal content. So the normal bit rate divided by the multiplier should be the bit rate for the I-frame. Dividing by a fraction is the same as multiplying by its inverse, so the result is 6.5 — the bit rate of a normal playlist of the same resolution times the fps of the I-frame playlist divided by eight.

### I-frame image sequences

I-frame image sequences using the `mjpg` codec have been added to support some third-party devices. The sequences should be low bandwidth and require minimal processing. Players should prefer video I-frame variants over image sequences.

The recommendations for image sequences are as folows:

- Supply a single `mjpg` variant

- Unencrypted

- 400 pixels wide with height based on the aspect ratio

- One key-frame every 1 to 2 seconds

- Bandwidth should be reasonable for the resolution based on the codec implementation

### Audio rendition groups and variants

In building up a multivariant playlist, the first step is to choose your video resolutions and codecs. These are your basic variants. Each one will have a video media playlist. The playlist URI may be repeated in multiple `EXT-X-STREAM-INF` tags so that the same video can be associated with different audio content.

You will have some set of audio languages and codecs. A particular codec may be in stereo, in 5.1 sound, or both. Create one audio group for each pair of codec and channel count. Each group needs to have every language in it.

When you’re making audio groups, there are some things to remember. First, ensure you have a stereo AAC group. This is good fallback because it’s something all devices can play. If you have multichannel in a lossless audio codec, it’s a good practice to have a multichannel AAC codec as well. Lossless requires a high bit rate. You want something available that has a lower bit rate. During playback you don’t want to switch the number of channels. If playback is in multichannel, you want to stay in multichannel.

Generally speaking, the player doesn’t switch between audio codecs, but there are three notable exceptions. The player switches between the AAC variants: AAC-LC, HE-AAC, HE-AACv2, and USAC (also called xHE-AAC). The player will also switch between lossless codecs and AAC codecs. In addition, when rendering audio to Spatial Audio-capable routes on Apple devices, the player may switch between available audio codecs and even channel layouts.

After you have your audio groups, you replicate the variant entries for each group, with some exceptions. If the codecs are switchable, like the AAC codecs, then you can spread the audio groups across the variants using the low audio bit rate group with the low video bit rates and the high audio bit rate group with the high video. But, if the codecs are not switchable, like AC-3 and lossless, then you want each codec to be associated with every variant. This doesn’t create new variant playlists; it just creates new `EXT-X-STREAM-INF` tags in the multivariant playlist, which associate a video playlist with an audio group.

You may encounter a problem where the variants you want to favor aren’t being chosen. The default behavior is to choose the highest bit rate among what’s currently playable. With USAC and with Dolby Digital Plus, this can cause an inversion where the chosen variant is not what you would prefer. To remedy this, Apple added the `SCORE` attribute. The value is a floating-point number. You have to put it on all the variants. If you want to set an order, it has to be complete, otherwise you’ll have situations where you won’t be able to choose. The usual filtering occurs to get down to a set of variants, any of which could be played. At that point, the system uses `SCORE` to decide and the highest `SCORE` wins.

### Values for the CODECS attribute

Use the `CODECS` attribute of the `EXT-X-STREAM-INF` tag (and `EXT-X-I-FRAME-STREAM-INF`) to specify media sample types. The value is a quoted-string containing a comma-separated list of formats, where each format specifies a media sample type that is present in a media segment of the playlist or in a media segment of some rendition that the tag references.

Valid format identifiers are those in the ISO Base Media File Format Name Space defined by RFC 6381. A format identifier is a sequence of elements separated by periods. The first element is the base sample type. HLS currently recognizes the following values for the base sample types:

| Base sample type | Description | Notes |
| --- | --- | --- |
| `ac-3` | AC-3 audio | |
| `alac` | Apple Lossless | |
| `apac` | Apple Positional Audio Codec | |
| `avc1` | H.264 (Advanced Video Coding) | |
| `avc3` | H.264 (Advanced Video Coding) | Use not recommended |
| `dvh1` | Dolby Vision (based on `hvc1`) | |
| `dvhe` | Dolby Vision (based on `hev1`) | Use not recommended |
| `ec-3` | Enhanced AC-3 audio | |
| `fLaC` | Free Lossless Audio Codec | |
| `hev1` | HEVC (High-Efficiency Video Coding) | Use not recommended |
| `hvc1` | HEVC (High-Efficiency Video Coding) | |
| `mjpg` | JPEG image sequence | Limited use |
| `mp4a` | MPEG-4 audio | |
| `stpp` | Subtitles (Timed Text) | |
| `wvtt` | WebVTT data | |

The MP4 registration authority ( mp4ra.org) lists a value of `ec+3` for Enhanced AC-3 audio with JOC (Dolby Atmos) but it has been deprecated now. HLS uses `ec-3` and marks the presence of the additional JOC content with `JOC` in the `CHANNELS` attribute of the audio rendition. The `JOC` must be capitalized. For example, `CHANNELS="16/JOC"`. The numeric value should match the value of the `complexity_index_type_a` field in the `EC3SpecificBox` of the Dolby Digital Plus audio track.

| Sample type | Description |
| --- | --- |
| `ac-3` | AC-3 audio |
| `alac` | Apple Lossless audio |
| `apac.31.00` | Apple Positional Audio Codec, profile 31, level 0 |
| `avc1.42001f` | H.264 Baseline Profile, Level 3.1 video |
| `avc1.4d0028` | H.264 Main Profile, Level 4.0 video |
| `avc1.640029` | H.264 High Profile, Level 4.1 video |
| `dvh1.05.01` | Dolby Vision Profile 5 (10-bit HEVC), Level 1 (720p24) video |
| `dvh1.05.06` | Dolby Vision Profile 5 (10-bit HEVC), Level 6 (2160p24) video |
| `ec-3` | Enhanced AC-3 audio |
| `fLaC` | Free Lossless Audio Codec audio |
| `hvc1.1.4.L126.B0` | HEVC Main Profile, Main Tier, Level 4.2 video |
| `hvc1.2.4.L123.B0` | HEVC Main 10 Profile, Main Tier, Level 4.1 video |
| `hvc1.2.4.L150.B0` | HEVC Main 10 Profile, Main Tier, Level 5.0 video |
| `mjpg` | JPEG image sequence |
| `mp4a.40.2` | AAC-LC audio |
| `mp4a.40.5` | HE-AAC audio |
| `mp4a.40.29` | HE-AACv2 audio |
| `mp4a.40.34` | MP3 audio |
| `mp4a.40.42` | xHE-AAC audio |
| `stpp.ttml.im1t` | IMSC1 text-only subtitles |
| `wvtt` | WebVTT subtitles |

### ALLOWED-CPC values for FairPlay Streaming

The `ALLOWED-CPC` attribute restricts playback of an encrypted variant stream to devices that guarantee a certain level of content protection robustness. The attribute associates a list of Content Protection Configuration (CPC) Labels with a specific `KEYFORMAT` value.

The permitted CPC Labels for FairPlay Streaming are:

| **CPC Label** | **Devices that conform to that CPC Label** |
| --- | --- |
| **AppleBaseline** | Any Apple platform that supports FairPlay Streaming. |
| **AppleMain** | Any Apple platform that supports FairPlay Streaming and guarantees enhanced content protection robustness (sufficient for studio 4K/HDR playback). |
| **Baseline** | Any non-Apple platform that supports FairPlay Streaming. For example, any AirPlay 2-enabled smart TV. |
| **Main** | Any non-Apple platform that supports FairPlay Streaming and guarantees enhanced content protection robustness (sufficient for studio 4K/HDR playback). |

An example of a valid attribute is: `ALLOWED-CPC="com.apple.streamingkeydelivery:AppleMain/Main"`

### The SUPPLEMENTAL-CODECS attribute

Some codecs are backward-compatible with other codecs. These codecs work by adding metadata that are ignored when being interpreted as the compatible codec, but used by the newer codec. These codecs include Dolby Vision 8.4 and 10.4 (compatible with HLG) and Dolby Vision 8.1 and 10.1 (compatible with HDR10).

To support these codecs on older implementations, the `CODECS` attribute is used to describe the base layer. The enhanced codec is described in the `SUPPLEMENTAL-CODECS` attribute. This allows implementations that support `SUPPLEMENTAL-CODECS` to take advantage of the true codec.

Each element in the `SUPPLEMENTAL-CODECS` attribute is a slash-separated list of fields. The first field must be a valid `CODECS` format. If more than one field is present, the remaining fields must be compatibility brands that pertain to that codec’s bitstream.

You can indicate the presence of HDR10+ metadata by adding a brand of ‘cdm4’.

Example-codec-values:

| **Codec** | **CODECS attribute** | **SUPPLEMENTAL-CODECS attribute** | **VIDEO-RANGE attribute** |
| --- | --- | --- | --- |
| Dolby Vision 8.4 | hvc1.2.4.L153.b0 | dvh1.08.07/db4h | HLG |
| Dolby Vision 8.1 | hvc1.2.4.L150 | dvh1.08.06/db1p | PQ |
| Dolby Vision 10.4 | av01.0.13M.10.0.112 | dav1.10.09/db4h | HLG |
| AV1 w/ HDR10+ | av01.0.05M.10.0.112 | av01.0.05M.10.0.112/cdm4 | PQ |

Note that, for Dolby Vision, the compatibility brand and the `VIDEO-RANGE` attribute act as cross-checks. Leaving out either one is incorrect.

### Dim Flashing Lights

Dim Flashing Lights is a setting (see What’s new in Accessibility) that allows people to indicate that they want to avoid bright, frequent flashes of light in video. As an additional measure, content producers can add markers to their HTTP Live Streaming content that identify the regions likely to cause discomfort.

Regions can be signalled using the standard `#EXT-X-DATERANGE` tag. The `CLASS` attribute should be set to “com.apple.accessibility.video.strobing.general-flash”. Add an additional `X-RISK-LEVEL` attribute. The risk level should be a decimal floating-point value in the range 0 to 100, where 0 is minimal risk and 100 is very risky.

To avoid using a large number of regions, restrict risk-level values to a small set of values. Use a risk level of zero for regions that have very low risk. Don’t mark regions with a risk level unless they have been analyzed. Raw risk values can be computed using an algorithm such as VideoFlashingReduction.

The `AVPlayerItemMetadataCollector` class can be used in your application to fetch the `#EXT-X-DATERANGE` tag metadata.

If you use the AVKit framework the metadata is fetched for you and the timeline is marked with a reddish color. If you display your own timeline you should do something similar.

### Additional spatial video specifications

Video Extended Usage atom ( `'vexu'`) is a sample description extension that conveys extensible information about spatial views. For more information, see ISO Base Media File Format and Apple HEVC Stereo Video.

Spatial video can benefit from frame based metadata. This can be provided using timed metadata tracks within ISOBMFF (ISO Base Media File Format) or QuickTime files.

You can provide parallax metadata for subtitles or captions using a timed metadata track. This allows control over the depth at which the text is displayed relative to the image. For details, see ISO Base Media File Format and Apple HEVC Stereo Video and Video Contour Map Payload Metadata within the QuickTime Movie File Format.

You can provide per frame rectangular mask metadata (PFRM, aka dynamic mask metadata) using a timed metadata track. This is used to indicate a fixed or changing rectangular area extracted from otherwise constant sized decoded video, for example letterboxing, or more complex spatial video adjustments to the displayed area. For details, see Rectangular Mask Payload Metadata within the QuickTime Movie File Format

Immersive video MUST point to an Apple Immersive Media Embedded (AIME) file via EXT-X-SESSION-DATA tag. This file provides information necessary to present the video correctly. To learn more about AIME, see Apple Immersive Media Embedded. See \[Apple Immersive Video Utility User Guide\] (https://support.apple.com/guide/immersive-video-utility/welcome/web) for more information.

Immersive video SHOULD use Apple Positional Audio Codec (APAC) for audio codec. APAC provides rich spatial audio experience. To learn more about APAC, see Apple Positional Audio Codec.

For more information on encoding MV-HEVC video, see Apple HEVC Stereo Video.

You can find also find these resources listed at AVFoundation Overview.

#### Multivariant Playlist and its resources expiry requirements

Content providers MUST assure that the original Multivariant Playlist URL and its resources do not expire on the CDN, as long as the downloaded asset will be needed by the application. There are 3 reasons.

- (Online playback) While online the player may attempt to load additional resources from the MVP (for assuring compatibility when the device configuration changes, e.g., an external display adapter is connected), which could cause play

- If the content supports Content Steering, Media Playlists MUST include STABLE-RENDITION-ID & STABLE-VARIANT-ID attributes; this decouples the variant identity from its CDN location.

- If one Media Playlist includes a STABLE-RENDITION-ID or STABLE-VARIANT-ID, all other Media Playlists MUST also specify a stable ID.

- The Content Steering manifest MUST remain available for the same timespan as the Multivariant Playlist URL above for the same reasons.

#### Interstitials requirements

- Your ads and other non-primary media MAY be inserted in the Media Playlists or as Interstitials.

- To allow predictable tier selection at the time of download, interstitial assets SHOULD follow the content structure of the main content (e.g., Codecs, subtitle/audio languages, etc.,).

#### Download performance requirements

- Download speed will be improved by authoring content in a way that reduces the total number of HTTP requests, and specifically the requests that have a short payload. HLS content intended for download SHOULD be encapsulated as fMP4 or elementary audio stream, and consecutive segments in Media Playlists use EXT-X-BYTERANGE attributes with contiguous ranges; this allows the number of HTTP requests to be reduced via coalescing. Content SHOULD also avoid usage of small files, where possible. For instance, subtitles can be authored as a single segment for all cues across the entire asset duration.

- Extra-long-form content, such as audiobooks, SHOULD be split in multiple assets (e.g., per chapter). This is particularly important for playback of downloaded audio assets on watchOS, to enable performant playback start-up and reduce battery usage.

#### Example playlist with Stereo video.

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=726521,BANDWIDTH=910558,VIDEO-RANGE=PQ,CODECS="dvh1.20.01,ac-3",RESOLUTION=640x360,FRAME-RATE=24.000,CLOSED-CAPTIONS=NONE,AUDIO="ac3-48-384",REQ-VIDEO-LAYOUT="CH-STEREO"
360p/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=7224756,BANDWIDTH=10079102,VIDEO-RANGE=PQ,CODECS="dvh1.20.01,ec-3",RESOLUTION=1280x720,FRAME-RATE=24.000,CLOSED-CAPTIONS=NONE,AUDIO="atmos-48-448",REQ-VIDEO-LAYOUT="CH-STEREO"
720p/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=12327020,BANDWIDTH=17120478,VIDEO-RANGE=PQ,CODECS="dvh1.20.03,ec-3",RESOLUTION=1920x1080,FRAME-RATE=24.000,CLOSED-CAPTIONS=NONE,AUDIO="atmos-48-448",REQ-VIDEO-LAYOUT="CH-STEREO"
1080p/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=16683700,BANDWIDTH=23228969,VIDEO-RANGE=PQ,CODECS="dvh1.20.05,ac-3",RESOLUTION=2560x1440,FRAME-RATE=24.000,CLOSED-CAPTIONS=NONE,AUDIO="ac3-48-384",REQ-VIDEO-LAYOUT="CH-STEREO"
1440p/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=34515644,BANDWIDTH=47959720,VIDEO-RANGE=PQ,CODECS="dvh1.20.06,ac-3",RESOLUTION=3840x2160,FRAME-RATE=24.000,CLOSED-CAPTIONS=NONE,AUDIO="ac3-48-384",REQ-VIDEO-LAYOUT="CH-STEREO"
2160p/prog_index.m3u8

#### Example playlist with APMP video.

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=25403063,BANDWIDTH=34135166,VIDEO-RANGE=SDR,CODECS="hvc1.2.20000000.H150.B0",RESOLUTION=3840x1920,FRAME-RATE=29.970,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-EQUI"
small/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=50285525,BANDWIDTH=65273029,VIDEO-RANGE=SDR,CODECS="hvc1.2.20000000.H180.B0",RESOLUTION=5440x2720,FRAME-RATE=29.970,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-EQUI"
med/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=102904567,BANDWIDTH=117277565,VIDEO-RANGE=SDR,CODECS="hvc1.2.20000000.H180.B0",RESOLUTION=7680x3840,FRAME-RATE=29.970,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-EQUI"
large/prog_index.m3u8

#EXT-X-I-FRAME-STREAM-INF:AVERAGE-BANDWIDTH=5070173,BANDWIDTH=6906054,VIDEO-RANGE=SDR,CODECS="hvc1.2.20000000.H180.B0",RESOLUTION=7680x3840,REQ-VIDEO-LAYOUT="CH-MONO/PROJ-RECT",URI="large/iframe_var.m3u8"

#### Example playlist with AIV video.

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=18077520,BANDWIDTH=30636545,AUDIO="apac",SUBTITLES="subs",VIDEO="stereo-16",VIDEO-RANGE=PQ,CODECS="hvc1.2.20000000.H183.B0,apac.31.00",RESOLUTION=3600x3600,FRAME-RATE=90.000,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-AIV"
Video/16Mb/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=21960196,BANDWIDTH=36415190,AUDIO="apac",SUBTITLES="subs",VIDEO="stereo-20",VIDEO-RANGE=PQ,CODECS="hvc1.2.20000000.H183.B0,apac.31.00",RESOLUTION=3600x3600,FRAME-RATE=90.000,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-AIV"
Video/20Mb/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=41505403,BANDWIDTH=71521624,AUDIO="apac",SUBTITLES="subs",VIDEO="stereo-40",VIDEO-RANGE=PQ,CODECS="hvc1.2.20000000.H183.B0,apac.31.00",RESOLUTION=4320x4320,FRAME-RATE=90.000,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-AIV"
Video/40Mb/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=98690153,BANDWIDTH=177339446,AUDIO="apac",SUBTITLES="subs",VIDEO="stereo-100",VIDEO-RANGE=PQ,CODECS="hvc1.2.20000000.H183.B0,apac.31.00",RESOLUTION=4320x4320,FRAME-RATE=90.000,CLOSED-CAPTIONS=NONE,REQ-VIDEO-LAYOUT="CH-STEREO/PROJ-AIV"
Video/100Mb/prog_index.m3u8

#### Example playlist with SDR, Dolby Vision, HDR10, and HLG content at resolutions from 720p to 4K

The SUPPLEMENTAL-CODECS attribute is used to indicate that the HDR10 content is compatible with Dolby Vison 8.1 and the HLG content is compatible with Dolby Vision 8.4.

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=2778321,BANDWIDTH=3971374,VIDEO-RANGE=SDR,CODECS="hvc1.2.4.L123.B0",RESOLUTION=1280x720,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=NONE
sdr_720/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=6759875,BANDWIDTH=10022043,VIDEO-RANGE=SDR,CODECS="hvc1.2.4.L123.B0",RESOLUTION=1920x1080,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-0
sdr_1080/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=20985770,BANDWIDTH=28058971,VIDEO-RANGE=SDR,CODECS="hvc1.2.4.L150.B0",RESOLUTION=3840x2160,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-1
sdr_2160/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=3385450,BANDWIDTH=5327059,VIDEO-RANGE=PQ,CODECS="dvh1.05.01",RESOLUTION=1280x720,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=NONE
dolby_720/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=7999361,BANDWIDTH=12876596,VIDEO-RANGE=PQ,CODECS="dvh1.05.03",RESOLUTION=1920x1080,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-0
dolby_1080/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=24975091,BANDWIDTH=30041698,VIDEO-RANGE=PQ,CODECS="dvh1.05.06",RESOLUTION=3840x2160,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-1
dolby_2160/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=3320040,BANDWIDTH=5280654,VIDEO-RANGE=PQ,CODECS="hvc1.2.4.L123.B0",SUPPLEMENTAL-CODECS="dvh1.08.01/db1p",RESOLUTION=1280x720,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=NONE
hdr10_dolby_720/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=7964551,BANDWIDTH=12886714,VIDEO-RANGE=PQ,CODECS="hvc1.2.4.L123.B0",SUPPLEMENTAL-CODECS="dvh1.08.03/db1p",RESOLUTION=1920x1080,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-0
hdr10_dolby_1080/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=24833402,BANDWIDTH=29983769,VIDEO-RANGE=PQ,CODECS="hvc1.2.4.L150.B0",SUPPLEMENTAL-CODECS="dvh1.08.08/db1p",RESOLUTION=3840x2160,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-1
hdr10_dolby_2160/prog_index.m3u8

#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=3061873,BANDWIDTH=3109758,VIDEO-RANGE=HLG,CODECS="hvc1.2.20000000.L150.B0",SUPPLEMENTAL-CODECS="dvh1.08.01/db4h",RESOLUTION=1280x720,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=NONE
hlg_dolby_720_24/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=6759750,BANDWIDTH=6884346,VIDEO-RANGE=HLG,CODECS="hvc1.2.20000000.L153.B0",SUPPLEMENTAL-CODECS="dvh1.08.03/db4h",RESOLUTION=1920x1080,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-0
hlg_dolby_1080_30/prog_index.m3u8
#EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=26472863,BANDWIDTH=28111779,VIDEO-RANGE=HLG,CODECS="hvc1.2.20000000.L183.B0",SUPPLEMENTAL-CODECS="dvh1.08.08/db4h",RESOLUTION=3840x2160,FRAME-RATE=23.976,CLOSED-CAPTIONS=NONE,HDCP-LEVEL=TYPE-1
hlg_dolby_2160_60/prog_index.m3u8

#EXT-X-I-FRAME-STREAM-INF:AVERAGE-BANDWIDTH=788595,BANDWIDTH=1777136,VIDEO-RANGE=HLG,CODECS="hvc1.2.20000000.L183.B0",SUPPLEMENTAL-CODECS="dvh1.08.08/db4h",RESOLUTION=3840x2160,HDCP-LEVEL=TYPE-1,URI="hlg_dolby_2160/prog_index.m3u8"

The HEVC codec values are described in ISO/IEC 14496-15. A short description is `Codec.Profile.Flags.TierLevel.Constraints`, so in `hvc1.2.4.L123.B0`, the `2` means _Main 10 profile_, and the `L123` means _normal tier, level 4.1_.

Information about Dolby Video codec values can be obtained from Dolby. A short description is `Codec.Profile.Level`, so in `dvh1.05.03` the Profile is 5 and the Level is 3.

---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices-appendixes).

.#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices).)



---

# https://developer.apple.com/documentation/http-live-streaming/hls-authoring-specification-for-apple-devices-appendixes)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/video-on-demand-playlist-construction

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming
- Video on Demand playlist construction

Article

# Video on Demand playlist construction

Understand the basic composition for a Video on Demand playlist.

## Overview

For Video on Demand (VOD) sessions, media files are available representing the entire duration of the presentation. The index file is static and contains a complete list of URLs to all media files created since the beginning of the presentation. This kind of session allows the client full access to the entire program.

### Example

This code is an example of a Video on Demand playlist:

#EXTINF:10.0,

#EXTINF:10.0,

#EXTINF:10.0,

#EXTINF:9.0,

#EXT-X-ENDLIST

These are the tags used in the Video on Demand playlist example:

**EXTM3U:** Indicates that the playlist is an extended M3U file. This type of file is distinguished from a basic `M3U` file by changing the tag on the first line to `EXTM3U`. All HLS playlists must start with this tag.

**EXT-X-PLAYLIST-TYPE:** Provides mutability information that applies to the entire playlist file. This tag may contain a value of either `EVENT` or `VOD`. If the tag is present and has a value of `EVENT`, the server must not change or delete any part of the playlist file (although it may append lines to it). If the tag is present and has a value of `VOD`, the playlist file must not change.

**EXT-X-TARGETDURATION:** Specifies the maximum media-file duration.

**EXT-X-VERSION:** Indicates the compatibility version of the playlist file. The playlist media and its server must comply with all provisions of the most recent version of the IETF Internet-Draft of the HTTP Live Streaming specification that defines that protocol version.

**EXT-X-MEDIA-SEQUENCE:** Indicates the sequence number of the first URL that appears in a playlist file. Each media file URL in a playlist has a unique integer sequence number. The sequence number of a URL is higher by 1 than the sequence number of the URL that preceded it. The media sequence numbers have no relation to the names of the files.

**EXTINF:** A record marker that describes the media file identified by the URL that follows it. Each media file URL must be preceded by an `EXTINF` tag. This tag contains a duration attribute that’s an integer or floating-point number in decimal positional notation that specifies the duration of the media segment in seconds. This value must be less than or equal to the target duration.

**EXT-X-ENDLIST:** Indicates that no more media files will be added to the playlist file.

The VOD playlist example above uses full pathnames for the media file playlist entries. While this is allowed, using relative pathnames is preferable. Relative pathnames are more portable than absolute pathnames and are relative to the URL of the playlist file. Using full pathnames for the individual playlist entries often results in more text than using relative pathnames. Here’s the same playlist with relative pathnames:

#EXTINF:10.0,
fileSequenceA.ts
#EXTINF:10.0,
fileSequenceB.ts
#EXTINF:10.0,
fileSequenceC.ts
#EXTINF:9.0,
fileSequenceD.ts
#EXT-X-ENDLIST

## See Also

### Basic playlists

Live Playlist (sliding window) construction

Understand the basic composition for a live session playlist.

Event playlist construction

Learn about the basic composition of an event session playlist.

Creating a Multivariant Playlist

Offer multiple playlist files to provide different encodings of the same content.

---

# https://developer.apple.com/documentation/http-live-streaming/live-playlist-sliding-window-construction

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming
- Live Playlist (sliding window) construction

Article

# Live Playlist (sliding window) construction

Understand the basic composition for a live session playlist.

## Overview

In live sessions, the index file is updated by removing media URIs from the file as new media files are created and made available. The `EXT-X-ENDLIST` tag isn’t present in the live playlist, indicating that new media files will be added to the index file as they become available.

### Example

This code is an example of a Live Playlist as it appears at the beginning of a session:

#EXTINF:10.0,
fileSequence1.ts
#EXTINF:10.0,
fileSequence2.ts
#EXTINF:10.0,
fileSequence3.ts
#EXTINF:10.0,
fileSequence4.ts
#EXTINF:10.0,
fileSequence5.ts

These are the tags used in the live playlist example:

**EXTM3U:** Indicates that the playlist is an extended M3U file. This type of file is distinguished from a basic M3U file by changing the tag on the first line to `EXTM3U`. All HLS playlists must start with this tag.

**EXT-X-TARGETDURATION:** Specifies the maximum media-file duration.

**EXT-X-VERSION:** Indicates the compatibility version of the playlist file. The playlist media and its server must comply with all provisions of the most recent version of the IETF Internet-Draft of the HTTP Live Streaming specification that defines that protocol version.

**EXT-X-MEDIA-SEQUENCE:** Indicates the sequence number of the first URL that appears in a playlist file. Each media file URL in a playlist has a unique integer sequence number. The sequence number of a URL is higher by 1 than the sequence number of the URL that preceded it. The media sequence numbers have no relation to the names of the files.

**EXTINF:** A record marker that describes the media file identified by the URL that follows it. Each media file URL must be preceded by an `EXTINF` tag. This tag contains a duration attribute that’s an integer or floating-point number in decimal positional notation that specifies the duration of the media segment in seconds. This value must be less than or equal to the target duration.

The following example shows the same playlist after it’s been updated with new media URIs:

#EXTINF:10.0,
#EXTINF:10.0,
fileSequence2.ts
fileSequence3.ts
#EXTINF:10.00,
#EXTINF:10.00,
fileSequence4.ts
fileSequence5.ts
#EXTINF:10.0,
fileSequence6.ts

The playlist continues to be updated as new media URIs are added:

#EXTINF:10.00,
#EXTINF:10.00,
#EXTINF:10.0,
fileSequence4.ts
fileSequence5.ts
fileSequence6.ts,
#EXTINF:10.0,
fileSequence7.ts,
#EXTINF:10.0,
fileSequence8.ts,
#EXTINF:10.0,
fileSequence9.ts

## See Also

### Basic playlists

Video on Demand playlist construction

Understand the basic composition for a Video on Demand playlist.

Event playlist construction

Learn about the basic composition of an event session playlist.

Creating a Multivariant Playlist

Offer multiple playlist files to provide different encodings of the same content.

---

# https://developer.apple.com/documentation/http-live-streaming/event-playlist-construction

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming
- Event playlist construction

Article

# Event playlist construction

Learn about the basic composition of an event session playlist.

## Overview

An event playlist is specified by the `EXT-X-PLAYLIST-TYPE` tag with a value of `EVENT`. It doesn’t initially have an `EXT-X-ENDLIST` tag, indicating that new media files will be added to the playlist as they become available.

### Example

The following code shows an example of an event playlist as it appears at the beginning of a session:

#EXTINF:10.00,
fileSequence0.ts
#EXTINF:10.0,
fileSequence1.ts
#EXTINF:10.0,
fileSequence2.ts
#EXTINF:10.0,
fileSequence3.ts
#EXTINF:10.0,
fileSequence4.ts

These are the tags used in the event playlist example:

**EXTM3U:** Indicates that the playlist is an extended M3U file. This type of file is distinguished from a basic M3U file by changing the tag on the first line to `EXTM3U`. All HLS playlists must start with this tag.

**EXT-X-PLAYLIST-TYPE:** Provides mutability information that applies to the entire playlist file. This tag may contain a value of either `EVENT` or `VOD`. If the tag is present and has a value of `EVENT`, the server must not change or delete any part of the playlist file (although it may append lines to it). If the tag is present and has a value of `VOD`, the playlist file must not change.

**EXT-X-TARGETDURATION:** Specifies the maximum media-file duration.

**EXT-X-VERSION:** Indicates the compatibility version of the playlist file. The playlist media and its server must comply with all provisions of the most recent version of the IETF Internet-Draft of the HTTP Live Streaming specification that defines that protocol version.

**EXT-X-MEDIA-SEQUENCE:** Indicates the sequence number of the first URL that appears in a playlist file. Each media file URL in a playlist has a unique integer sequence number. The sequence number of a URL is higher by 1 than the sequence number of the URL that preceded it. The media sequence numbers have no relation to the names of the files.

**EXTINF:** A record marker that describes the media file identified by the URL that follows it. Each media file URL must be preceded by an EXTINF tag. This tag contains a duration attribute that’s an integer or floating-point number in decimal positional notation that specifies the duration of the media segment in seconds. This value must be less than or equal to the target duration.

You can’t remove anything from the playlist when using the `EVENT` tag; you may only append new segments to the end of the file. New segments are added to the end of the file until the event has concluded, at which time the `EXT-X-ENDLIST` tag is appended. The following example shows the same playlist after it’s been updated with new media URIs and the event has ended:

#EXTINF:10.0,
#EXTINF:10.0,
fileSequence0.ts
fileSequence1.ts
#EXTINF:10.0,
#EXTINF:10.0,
fileSequence2.ts
fileSequence3.ts
#EXTINF:10.0,

// List of files between 4 and 120 go here.

#EXTINF:10.0,
fileSequence120.ts
#EXTINF:10.0,
fileSequence121.ts
#EXT-X-ENDLIST

Event playlists are typically used when you want to allow the user to seek to any point in the event, such as for a concert or sports event.

## See Also

### Basic playlists

Video on Demand playlist construction

Understand the basic composition for a Video on Demand playlist.

Live Playlist (sliding window) construction

Understand the basic composition for a live session playlist.

Creating a Multivariant Playlist

Offer multiple playlist files to provide different encodings of the same content.

---

# https://developer.apple.com/documentation/http-live-streaming/creating-a-multivariant-playlist

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming
- Creating a Multivariant Playlist

Article

# Creating a Multivariant Playlist

Offer multiple playlist files to provide different encodings of the same content.

## Overview

The Multivariant Playlist describes all of the available variants for your content. Each variant is a version of the stream at a particular bit rate and is contained in a separate playlist. The client switches to the most appropriate variant based on the measured network bit rate. The client’s player is tuned to minimize stalling of playback, to give the user the best possible streaming experience.

A Multivariant Playlist isn’t re-read. Once the client has read the playlist, it assumes the set of variations isn’t changing. The stream ends as soon as the client sees the `EXT-X-ENDLIST` tag on one of the individual variant playlists.

### Define variants

The following example shows a Multivariant Playlist that defines five different variants.

#EXT-X-STREAM-INF:BANDWIDTH=150000,RESOLUTION=416x234,CODECS="avc1.42e00a,mp4a.40.2"

#EXT-X-STREAM-INF:BANDWIDTH=240000,RESOLUTION=416x234,CODECS="avc1.42e00a,mp4a.40.2"

#EXT-X-STREAM-INF:BANDWIDTH=440000,RESOLUTION=416x234,CODECS="avc1.42e00a,mp4a.40.2"

#EXT-X-STREAM-INF:BANDWIDTH=640000,RESOLUTION=640x360,CODECS="avc1.42e00a,mp4a.40.2"

#EXT-X-STREAM-INF:BANDWIDTH=64000,CODECS="mp4a.40.5"

The tags used in the playlist example are:

`EXTM3U`

Indicates that the playlist is an extended M3U file. This type of file is distinguished from a basic M3U file by changing the tag on the first line to `EXTM3U`. All HLS playlists must start with this tag.

`EXT-X-STREAM-INF`

Indicates that the next URL in the playlist file identifies another playlist file.

The `EXT-X-STREAM-INF` tag has the following parameters:

`AVERAGE-BANDWIDTH`

(Optional, but recommended) An integer that represents the average bit rate for the variant stream.

`BANDWIDTH`

(Required) An integer that is the upper bound of the overall bit rate for each media file, in bits per second. The upper bound value is calculated to include any container overhead that appears or will appear in the playlist.

`FRAME-RATE`

(Optional, but recommended) A floating-point value that describes the maximum frame rate in a variant stream.

`HDCP-LEVEL`

(Optional) Indicates the type of encryption used. Valid values are `TYPE-0` and `NONE`. Use `TYPE-0` if the stream may not play unless the output is protected by HDCP.

`RESOLUTION`

(Optional, but recommended) The optional display size, in pixels, at which to display the video in the playlist. This parameter should be included for any stream that includes video.

`VIDEO-RANGE`

(Required depending on encoding) A string with valid values of `SDR` or `PQ`. If transfer characteristic codes 1, 16, or 18 aren’t specified, then this parameter must be omitted.

`CODECS`

(Optional, but recommended) A quoted string containing a comma-separated list of formats, where each format specifies a media sample type that’s present in a media segment in the playlist file. Valid format identifiers are those in the ISO file format name space defined by RFC 6381.

## See Also

### Basic playlists

Video on Demand playlist construction

Understand the basic composition for a Video on Demand playlist.

Live Playlist (sliding window) construction

Understand the basic composition for a live session playlist.

Event playlist construction

Learn about the basic composition of an event session playlist.

---

# https://developer.apple.com/documentation/http-live-streaming/incorporating-ads-into-a-playlist

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming
- Incorporating Ads into a Playlist

Article

# Incorporating Ads into a Playlist

Add branding or ads to a playlist.

## Overview

Often you want to deliver a series of movies with some sort of branding (advertisement) displayed in front of each one to let the user know that they originate from your site. One way to do this is to simply merge the ad with each movie. However, if you have hundreds of movies, you’ll have to redo a lot of encoding, and you’ll be duplicating the ad with each movie.

You could deliver the ad as a separate movie that plays first, and then play the intended movie. The problem with that approach, however, is that quality drops during the transition from the ad to the movie. For example, the ad starts playing with a low data rate to ensure that the client can read it, then gradually ramps up to provide the best possible playback experience. When the ad is finished playing, the movie starts at a low data rate (just as the ad did) and ramps up, resulting in a break in quality. Also, if you display the ad in the middle of the movie, you’ll get ongoing drops in quality.

The solution is to let the client know a change is coming, by using the `EXT-X-DISCONTINUITY` tag. This tag informs the client of a change that’s coming to the streaming media so the client can prepare for the change ahead of time.

### Example

The following example shows a stream that uses the `EXT-X-DISCONTINUITY` tag to play movies that are preceded by an 18-second ad (segments `ad0.ts` and `ad1.ts`):

#EXTINF:10.0,
ad0.ts
#EXTINF:8.0,
ad1.ts
#EXTINF:10.0,
movieA.ts
#EXTINF:10.0,
movieB.ts

These are the tags used in the ads playlist example:

**EXTM3U:** Indicates that the playlist is an extended M3U file. This type of file is distinguished from a basic M3U file by changing the tag on the first line to EXTM3U. All HLS playlists must start with this tag.

**EXT-X-TARGETDURATION:** Specifies the maximum media-file duration.

**EXT-X-VERSION:** Indicates the compatibility version of the playlist file. The playlist media and its server must comply with all provisions of the most recent version of the IETF Internet-Draft of the HTTP Live Streaming specification that defines that protocol version.

**EXT-X-MEDIA-SEQUENCE:** Indicates the sequence number of the first URL that appears in a playlist file. Each media file URL in a playlist has a unique integer sequence number. The sequence number of a URL is higher by 1 than the sequence number of the URL that preceded it. The media sequence numbers have no relation to the names of the files.

**EXT-X-DISCONTINUITY:** Indicates an encoding discontinuity between the media file that follows it and the one that preceded it.

**EXT-X-DISCONTINUITY-SEQUENCE:** Provides synchronization between different variant streams or different renditions of the same variant stream. You must use this tag for live events that have discontinuities.

**EXTINF:** A record marker that describes the media file identified by the URL that follows it. Each media file URL must be preceded by an `EXTINF` tag. This tag contains a duration attribute that’s an integer or floating-point number in decimal positional notation that specifies the duration of the media segment in seconds. This value must be less than or equal to the target duration.

## See Also

### Modified playlists

Adding alternate media to a playlist

Specify Rendition Playlists that can override the main presentation.

---

# https://developer.apple.com/documentation/http-live-streaming/adding-alternate-media-to-a-playlist

- HTTP Live Streaming
- Example playlists for HTTP Live Streaming
- Adding alternate media to a playlist

Article

# Adding alternate media to a playlist

Specify Rendition Playlists that can override the main presentation.

## Overview

Adding alternate media to a Multivariant Playlist allows a provider to specify one of a set of variant playlists as an _override_ of the main presentation. The client plays only the override media (audio or video), and suppresses any media of the same type from the main presentation, if present. This allows a presentation to offer multiple versions of the media without requiring the provider to store duplicate media, or requiring the client to download all variants when it only needs one. It also allows additional media to be offered subsequently without remastering the original content.

### Add alternate media

Here’s an example of a Multivariant Playlist that provides additional audio renditions:

#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=195023,CODECS="avc1.42e00a,mp4a.40.2",AUDIO="audio"
lo/prog_index.m3u8
#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=591680,CODECS="avc1.42e01e,mp4a.40.2",AUDIO="audio"
hi/prog_index.m3u8

The tags used in this Multivariant Playlist example include:

`EXT-X-MEDIA`

Identifies an element of a media selection group. All the elements of a media selection group must have similar characteristics, for example, the same codecs and the same maximum bandwidth.

`EXT-X-STREAM-INF`

indicates that the next URL in the Multivariant Playlist identifies a Rendition Playlist. See Creating a Multivariant Playlist for the basic parameters.

The EXT-X-MEDIA tag has the following parameters:

`TYPE`

(Required) A string indicating the type of media. Valid values are `AUDIO`, `VIDEO`, `SUBTITLES`, and `CLOSED-CAPTIONS`.

`GROUP-ID`

(Required) A string specifying the group that the media selection belongs to.

`LANGUAGE`

(Optional) A string that identifies the primary language used in the media selection.

`NAME `

(Required) A string that describes the primary language used in the media selection.

`AUTOSELECT`

(Optional) A string that indicates that the client may play the media selection in the absence of explicit user preference. Valid values are `YES` and `NO`. If the value of `DEFAULT` is `YES`, this value must also be `YES`.

`DEFAULT`

(Optional) A string indicating that the media selection should be played if the user hasn’t selected another option. Valid values are `YES` and `NO`.

`INSTREAM-ID`

(Required for closed captions) A string that specifies a rendition within the segments in the media playlist. When the `TYPE` attribute is `CLOSED-CAPTIONS`, the `INSTREAM-ID` must have one of the following values: `CC1`, `CC3`, `CC3`, `CC4`, or `SERVICEn`, where `n` is between 1 and 63.

`ASSOC-LANGUAGE`

(Optional) A string containing a language tag for the rendition. An associated language is often different from the language specified in the `LANGUAGE` attribute.

`CHANNELS`

(Required when two renditions have the same codec but a different number of channels) An ordered string that indicates the maximum number of independent, simultaneous audio channels present in a media segment.

`URI`

(Optional) A string containing a URI that identifies the media playlist file. If the `TYPE` is `CLOSED-CAPTIONS`, this attribute must be omitted. When this attribute is omitted, the media content is in the original variant.

When its URI attribute is omitted, the `EXT-X-MEDIA` tag can indicate that the media described is included in the URI of the `EXT-X-STREAM-INF` tag.

The `EXT-X-STREAM-INF` tag has the following parameters:

`AUDIO`

(Optional) A quoted string that indicates the set of audio streams that may be used when playing the presentation. This value must match the value of the `GROUP-ID` attribute of an `EXT-X-MEDIA` tag elsewhere in the Multivariant Playlist whose `TYPE` attribute is `AUDIO`.

`VIDEO`

(Optional) A quoted string that indicates the set of video streams that may be used when playing the presentation. This value must match the value of the `GROUP-ID` attribute of an `EXT-X-MEDIA` tag elsewhere in the Multivariant Playlist whose `TYPE` attribute is `VIDEO`.

`SUBTITLES`

(Optional) A quoted string that indicates the set of subtitle renditions that can be used. This value must match the value of the `GROUP-ID` attribute of an `EXT-X-MEDIA` tag elsewhere in the Multivariant Playlist whose `TYPE` attribute is `SUBTITLE`.

`CLOSED-CAPTIONS`

(Optional) Either a quoted string that indicates the set of closed captions that can be used or an enumerated string with the value of `NONE`. When this value is a quoted string, it must match the value of the `GROUP-ID` attribute of an `EXT-X-MEDIA` tag elsewhere in the Multivariant Playlist whose `TYPE` attribute is `CLOSED-CAPTIONS`. If the enumerated value is `NONE`, all `EXT-X-STREAM-INF` tags must have this attribute with a value of `NONE`.

You can have multiple audio groups to allow changes in codes or bit rate. However, each audio group in a variant must have the same alternates in it. For example, you can’t have English in one audio group and leave it out of the other group. The following example defines two audio groups, one for low bit rates and one for high bit rates. Both audio groups define the same set of languages but are called based on the available bandwidth.

#EXT-X-STREAM-INF:BANDWIDTH=195023,CODECS="mp4a.40.5",AUDIO="audio-lo"
#EXT-X-STREAM-INF:BANDWIDTH=260000,CODECS="avc1.42e01e,mp4a.40.2",AUDIO="audio-lo"
lo/prog_index.m3u8
hi/prog_index.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=591680,CODECS="mp4a.40.2,avc1.64001e",AUDIO="audio-hi"
#EXT-X-STREAM-INF:BANDWIDTH=650000,CODECS="avc1.42e01e,mp4a.40.2",AUDIO="audio-hi"

### Combine Groups and Single Options

You can have both a group and a single stream in a playlist. This is often done when you have multiple camera angles that all use the same audio. Create a group for the video streams and then declare the single audio stream. The following example shows a playlist with three camera angles and a single audio stream:

#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=754857,CODECS="mp4a.40.2,avc1.4d401e",VIDEO="500kbs",AUDIO="aac"
Angle1/500kbs/prog_index.m3u8

To provide different streams for different bit rates, a different video group ID is needed for each bit rate.

#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=300000,CODECS="mp4a.40.2,avc1.4d401e",VIDEO="200kbs",AUDIO="aac"
Angle1/200kbs/prog_index.m3u

#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=754857,CODECS="mp4a.40.2,avc1.4d401e",VIDEO="500kbs",AUDIO="aac"

## See Also

### Modified playlists

Incorporating Ads into a Playlist

Add branding or ads to a playlist.

---

# https://developer.apple.com/documentation/http-live-streaming/video-on-demand-playlist-construction)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/live-playlist-sliding-window-construction)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/event-playlist-construction)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/creating-a-multivariant-playlist)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/incorporating-ads-into-a-playlist)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/http-live-streaming/adding-alternate-media-to-a-playlist)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

