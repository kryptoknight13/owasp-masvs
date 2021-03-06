# V6: Environmental interaction requirements

## Control objective

The controls in group this ensure that the app uses operation system APIs and standard components in a secure manner. Additionally, the controls cover communication between apps (IPC).

## Requirements

| # | Description | L1 | L2 | L3 | L4 |
| --- | --- | --- | --- | --- | --- |
| **6.1** | Verify that that the app does not request any unnecessary permissions. | ✓ | ✓ | ✓ | ✓ |
| **6.2** | Verify that all inputs from external sources is validated. This includes data received via the GUI, IPC mechanisms such as intents, custom URLs, and network communication.| ✓ | ✓ | ✓ | ✓ |
| **6.3** | Verify that all user input is sanitized and verified (both when using input fields, as well as barcode/QR code data, NFC-related data, etc.).| ✓ | ✓ | ✓ | ✓ |
| **6.4** | Verify that the app does not export sensitive functionality via custom URL schemes. | ✓ | ✓ | ✓ | ✓ |
| **6.5** | Verify that the app does not export sensitive functionality through IPC facilities. | ✓ | ✓ | ✓ | ✓ |
| **6.6** | Verify that Javascript is disabled in all WebViews unless explicitly required. | ✓ | ✓ | ✓ | ✓ |
| **6.7** | Verify that file access is disabled in all WebViews unless explicitly required. | ✓ | ✓ | ✓ | ✓ |
| **6.8** | If Javascript is required in a WebView, ensure that the WebView is restricted to a specific URL, and that no unfiltered user input is rendered in the WebView. | ✓ | ✓ | ✓ | ✓ |
| **6.9** | Verify that the app does not load user-supplied local resources into WebViews. | ✓ | ✓ | ✓ | ✓ |
| **6.10** | If Java objects are exposed in a WebView, verify that the WebView only renders JavaScript contained within the APK (Android). | ✓ | ✓ | ✓ | ✓ |
| **6.11** | Verify that the app leverages operating system features that allow updating of outdated system components. |   | ✓ | ✓ | ✓ |
| **6.12** | Verify that the app provides a custom keyboard whenever sensitive data is entered. |   |   | ✓ | ✓ |
| **6.13** | Verify that custom ui-components are used when sensitive data is displayed. The UI-component should not rely on immutable data structures. |   |   | ✓ | ✓ |


## References

For more information, see also:

- OWASP Mobile Top 10:  M1 - Improper Platform Usage: https://www.owasp.org/index.php/Mobile_Top_10_2016-M1-Improper_Platform_Usage
- CWE: https://cwe.mitre.org/data/definitions/20.html
- CWE: https://cwe.mitre.org/data/definitions/749.html
