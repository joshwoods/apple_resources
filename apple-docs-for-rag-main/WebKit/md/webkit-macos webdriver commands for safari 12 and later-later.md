

- WebKit
-  macOS WebDriver Commands for Safari 12 and later 

Article

# macOS WebDriver Commands for Safari 12 and later

Test your web content using the WebDriver commands supported by Safari 12 and later.

## Overview

This table lists the method and the URI template (the *endpoint*) that executes each command. The macOS WebDriver Commands for Safari 11.1 and earlier support the Selenium JSON Wire Protocol. The macOS WebDriver Commands for Safari 12 and later support the the W3C WebDriver protocol.

All URI templates listed here are supported by the `safaridriver` tool included with Safari 12 and later. For more information on the tool, see About WebDriver for Safari.

| Method | URI template | Supported | Safari Technology Preview release, Safari version |
|----|----|----|----|
| POST | /session | ✓ | 60, 12 |
| DELETE | /session/{session id} | ✓ | 60, 12 |
| GET | /status | ✓ | 60, 12 |
| GET | /session/{session id}/timeouts | ✓ | 60, 12 |
| POST | /session/{session id}/timeouts | ✓ | 60, 12 |
| POST | /session/{session id}/url | ✓ | 60, 12 |
| GET | /session/{session id}/url | ✓ | 60, 12 |
| POST | /session/{session id}/back | ✓ | 60, 12 |
| POST | /session/{session id}/forward | ✓ | 60, 12 |
| POST | /session/{session id}/refresh | ✓ | 60, 12 |
| GET | /session/{session id}/title | ✓ | 60, 12 |
| GET | /session/{session id}/window | ✓ | 60, 12 |
| DELETE | /session/{session id}/window | ✓ | 60, 12 |
| POST | /session/{session id}/window | ✓ | 60, 12 |
| GET | /session/{session id}/window/handles | ✓ | 60, 12 |
| POST | /session/{session id}/frame | ✓ | 60, 12 |
| POST | /session/{session id}/frame/parent | ✓ | 60, 12 |
| GET | /session/{session id}/window/rect | ✓ | 60, 12 |
| POST | /session/{session id}/window/rect | ✓ | 60, 12 |
| POST | /session/{session id}/window/maximize | ✓ | 60, 12 |
| POST | /session/{session id}/window/maximize | ✓ | 60, 12 |
| POST | /session/{session id}/window/fullscreen | ✓ | 60, 12 |
| GET | /session/{session id}/element/active | ✓ | 60, 12 |
| POST | /session/{session id}/element | ✓ | 60, 12 |
| POST | /session/{session id}/elements | ✓ | 60, 12 |
| POST | /session/{session id}/element/{element id}/element | ✓ | 60, 12 |
| POST | /session/{session id}/element/{element id}/elements | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/selected | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/attribute/{name} | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/property/{name} | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/css/{property name} | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/text | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/name | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/rect | ✓ | 60, 12 |
| GET | /session/{session id}/{element id}/enabled | ✓ | 60, 12 |
| POST | /session/{session id}/element/{element id}/click | ✓ | 60, 12 |
| POST | /session/{session id}/element/{element id}/clear | ✓ | 60, 12 |
| POST | /session/{session id}/element/{element id}/value | ✓ | 60, 12 |
| GET | /session/{session id}/source | ✓ | 60, 12 |
| POST | /session/{session id}/execute/sync | ✓ | 60, 12 |
| POST | /session/{session id}/execute/async | ✓ | 60, 12 |
| GET | /session/{session id}/cookie | ✓ | 60, 12 |
| GET | /session/{session id}/cookie/{name} | ✓ | 60, 12 |
| POST | /session/{session id}/cookie | ✓ | 60, 12 |
| DELETE | /session/{session id}/cookie/{name} | ✓ | 60, 12 |
| DELETE | /session/{session id}/cookie | ✓ | 60, 12 |
| POST | /session/{session id}/actions | ✓ | 60, 12 |
| DELETE | /session/{session id}/actions | ✓ | 60, 12 |
| POST | /session/{session id}/alert/dismiss | ✓ | 60, 12 |
| POST | /session/{session id}/alert/accept | ✓ | 60, 12 |
| GET | /session/{session id}/alert/text | ✓ | 60, 12 |
| POST | /session/{session id}/alert/text | ✓ | 60, 12 |
| GET | /session/{session id}/screenshot | ✓ | 60, 12 |
| GET | /session/{session id}/element/{element id}/screenshot | ✓ | 60, 12 |

## See Also

### WebDriver

macOS WebDriver Commands for Safari 11.1 and earlier

Test your web content using the WebDriver commands supported by Safari 11.1 and earlier.

About WebDriver for Safari

Enhance testing of your web content using Safari’s enhancements to WebDriver.

Testing with WebDriver in Safari

Enable WebDriver and run a test.

