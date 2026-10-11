# ME Control Web v1.1 (iPhone-friendly prototype)

This is a static web app/PWA prototype and does not require a Mac to preview.

## Interface
- Home screen: `#l` (Koti), `#ly` (Ylläpito), `#l` (Päälle), `OFF` (Pois päältä), temperature control using `Hxx`, and a `STATUS?` query button.
- Settings page: phone number and editable local drafts for four SET commands.
- No separate fan tab, no separate query tab, and no manually saved SMS acknowledgments.

## How to use on iPhone
For an installable Home Screen web app, these files must be hosted at an HTTPS address. Upload all files to a static host, open the HTTPS URL in Safari, tap Share, then Add to Home Screen.

## SMS limitations
- Tapping a command opens the iPhone Messages composer with recipient and message prefilled; the user must confirm/send.
- The response to `STATUS?` arrives in the regular Messages app. This web app does not attempt to read incoming SMS.
- `#l`, `#ly`, `OFF`, `STATUS?`, and `Hxx` are the commands agreed in the conversation. Verify them on the real controller before use.
- SET editor is a local draft. The displayed SET syntax must be verified against the exact ME Control manual before sending. The current prototype limits SET temperature to 16–31 °C and keeps the existing `#ly` command for the 12 °C maintenance mode.
- Fan values remain editable inside SET drafts, but there is no separate fan tab or standalone fan command.
