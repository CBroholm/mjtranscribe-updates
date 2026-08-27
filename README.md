# MjTranscribe updates

This repo is **not** the app. It exists only so MjTranscribe's colleague-beta
build can check "is there a newer version?" from any machine, without
depending on a machine-specific local file path (see the main repo's
[PRD #51](https://github.com/CBroholm/Mj-Transcribe/issues/51) for why).

It holds exactly one file, `version.json`, written by the main repo's
`publish.ps1 -BetaRelease`. It is deliberately public: the file has no
secrets and no application code, only a version number and a timestamp.

**The actual application build is never published here.** It lives in
Mjølner's internal shared OneDrive/SharePoint folder — this repo only tells
a beta install whether it's worth going to fetch a newer one from there.
