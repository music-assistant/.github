# Music Assistant - Usage Policy

Music Assistant plays the music you already have access to, on the speakers you own. It connects to streaming services using your own account, and to your own local files, and sends that audio to players on your own network.

It is not a tool for downloading, extracting, or keeping copies of music, and we do not build features that would make it one.

## What this means in practice

Music Assistant is designed so that audio flows to your speakers and stops there:

- **No interface hands out a provider's audio.** Nothing in the API, and no endpoint, returns a streaming service's own audio URL. The address a provider gives us is used to fetch audio and is never passed on.
- **Playback addresses are temporary.** The URL a player uses belongs to one playback session and stops working when that session ends.
- **Audio is delivered for listening, not collecting.** Audio is served at a rate that suits playback, and is never written to disk.
- **We respect each service's limits.** Where a service states how many streams an account may run at once, Music Assistant holds itself to that number.
- **We do not work around copy protection.** Content protected by DRM is skipped rather than decoded, and we will not accept changes that circumvent it.
- **We do not fetch what nobody asked to hear.** Background processing such as audio analysis is limited to your own files and never pulls a streaming service's catalogue.

## What we ask of you

Use Music Assistant with your own accounts and your own music, and within the terms of the services you have subscribed to. Do not use it to obtain, keep, or pass on music you do not have the right to.

Please do not ask us to add downloading, exporting, or archiving features. Requests of that kind are declined as a matter of policy rather than on technical merit, and we will close them.

## What we ask of contributors

Contributions that connect Music Assistant to a music service must fetch audio as an ordinary client would, using the account the user has provided. Do not add code that circumvents copy protection, bypasses a subscription tier or regional availability, stores decoded audio, or exposes a provider's audio address to anything outside the server.

Project-specific guidance for provider development lives in the [server repository](https://github.com/music-assistant/server/blob/dev/DEVELOPMENT.md).

## An honest limit

Music Assistant is open source and runs on hardware you control. Anyone can change their own copy of it, and nothing here prevents that. The measures above state our intent and prevent casual misuse; they are not a content protection system and we do not present them as one. This is the same position as any other open source media player.

What we can control is what the project ships, what we accept into it, and what we support. On all three, the answer is the same: Music Assistant is for listening to your own music.

## Enforcement

We do not provide help with using Music Assistant to obtain music you do not have access to, and discussion of doing so is off topic in our community spaces. Persisting with it may result in being removed from those spaces or blocked from contributing to Open Home Foundation projects.
