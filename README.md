# Privacy Policy – YouTube AI Chapters

_Last updated: July 16, 2026_

YouTube AI Chapters is a browser extension that generates clickable chapters for YouTube videos that do not have official chapters. Protecting your privacy is a core design goal of this extension.

## What data the extension processes

**The extension does not collect, store, transmit or sell any personal data.** There are no analytics, no tracking, no accounts and no server operated by the developer.

The only data that may leave your device is the **publicly available transcript of the YouTube video** you are watching. It is sent to exactly one AI service in order to generate chapter titles, depending on your settings:

| AI source | Data sent | Where it goes |
|---|---|---|
| Chrome built-in AI (Gemini Nano) | nothing leaves your device | processed locally in your browser |
| Local algorithm | nothing leaves your device | processed locally in your browser |
| Google Gemini (your own API key) | video transcript | generativelanguage.googleapis.com (Google) |
| Anthropic Claude (your own API key) | video transcript | api.anthropic.com (Anthropic) |
| Free cloud AI | video transcript | text.pollinations.ai (Pollinations) or api.llm7.io (LLM7) |

The transcript contains no information about you – it is the same public caption data anyone can see on the video's page.

## Data stored locally

The extension stores the following data **only on your device** using Chrome's extension storage (`chrome.storage.local`):

- Your settings (AI source, chapter granularity, filters)
- Your optional API key (used exclusively for requests to the provider it belongs to; never sent anywhere else)
- Generated chapters per video (cache, so chapters don't need to be regenerated)

You can delete the chapter cache at any time via the extension popup ("Clear cache"). Removing the extension deletes all stored data.

## Permissions

- **youtube.com access**: required to read the video transcript and display the chapter UI on YouTube watch pages.
- **storage**: required to save your settings and the chapter cache locally.
- **offscreen / scripting**: required for Chrome's built-in AI and to (re-)load the extension's own scripts on YouTube tabs. Not used to access any other websites.
- **AI service hosts** (googleapis.com, anthropic.com, pollinations.ai, llm7.io): required solely to send the video transcript for chapter generation, as described above.

## Third-party services

When a cloud AI source is used, the video transcript is processed by the respective provider under their own terms and privacy policies (Google, Anthropic, Pollinations, LLM7). If you prefer that no data leaves your device, select "Chrome AI only" or "Local algorithm only" in the extension options.

## Changes

If this policy changes, the updated version will be published at the same location as this document and the "Last updated" date will be revised.

## Contact

For privacy-related questions, contact: leon.lh76@gmail.com
