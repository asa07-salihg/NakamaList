# Privacy Policy

**App:** NakamaList  
**Effective date:** June 6, 2026  
**Maintainer:** Ahmet Salih Gölen  
**Contact:** nakamalist@proton.me

NakamaList ("the App", "we", "us") is an independent, mobile-first Android client
for the MyAnimeList community. This Privacy Policy explains what data the App
accesses, how it is used, and how it is stored. NakamaList is not affiliated with,
endorsed by, or officially connected to MyAnimeList Co., Ltd.

## Summary

- NakamaList has **no backend server**, so your app data stays on your device.
- We **never see, store, inspect, or log your MyAnimeList password**.
- Sign-in uses MyAnimeList's official OAuth 2.0 flow where available.
- Some MyAnimeList community features may open inside an **in-app WebView fallback**
  when official APIs are unavailable or incomplete.
- We do **not** sell, rent, or share your personal data with third parties.
- Network requests are made only to services required for app functionality, such as
  MyAnimeList services, optional metadata providers used by the App, and content
  sources needed to display images, news, or web fallback pages.
- The App contains **no third-party analytics, tracking, or advertising SDKs**.

## Information the App Accesses

When you sign in with your MyAnimeList account, the App accesses (through the
official MyAnimeList API and only to provide app features) data such as:

- Your MyAnimeList profile information, including username, profile details, and statistics.
- Your anime and manga lists, scores, statuses, and progress.
- Forum boards, topics, and replies you view where supported by the official API.
- Club, news, and other community content you browse.
- Account-related data required to keep you signed in and synchronize supported features.

The App requests only the access needed to provide its features.

## Authentication and Tokens

- Sign-in uses MyAnimeList's OAuth 2.0 Authorization Code flow with PKCE where available.
- The App may receive an **access token** and a **refresh token** from MyAnimeList.
- These tokens are stored securely on your device using Android platform security
  features, such as Android Keystore-backed encrypted storage.
- Your MyAnimeList username and password are entered only on MyAnimeList-controlled
  pages, such as the official OAuth page or MyAnimeList web pages opened for fallback.
- NakamaList does not receive, store, inspect, or log your MyAnimeList password.
- Tokens are never written to logs, crash reports, analytics services, or any remote
  service operated by NakamaList.

## Web Fallback / In-App WebView

Some MyAnimeList community features may not be available through the official
MyAnimeList API, or the available API may be incomplete for the feature being used.
When this happens, NakamaList may open the relevant MyAnimeList web page inside an
in-app WebView fallback.

The WebView is used only as an interactive browser surface so that you can use the
relevant MyAnimeList page directly. NakamaList does **not** use the WebView to:

- Scrape MyAnimeList pages.
- Parse web page HTML into native app data.
- Extract cookies or session tokens.
- Read, inspect, or store your password.
- Auto-submit hidden forms.
- Perform hidden actions on your behalf.
- Reuse MyAnimeList web page contents as an internal data source.

If you sign in to MyAnimeList inside the WebView, that web session is handled by
MyAnimeList and by the Android WebView/browser storage on your device. You can clear
this state by logging out from MyAnimeList inside the WebView, clearing the App's
local data, or uninstalling the App.

## Data Storage

All data the App stores is kept **locally on your device**, including:

- Authentication tokens, stored securely.
- Cached anime, manga, forum, club, and news content for offline access and speed.
- App preferences, such as language, theme, fallback mode, news refresh interval,
  and similar settings.
- News read/unread and bookmark state.
- WebView/browser storage used by Android WebView for pages you open inside the App.

NakamaList does not operate backend servers and does not upload, back up, or process
your app data on NakamaList-controlled servers.

Any statistics or charts the App shows about your own lists (such as the score, genre,
and format breakdowns on the Profile screen) are **computed locally on your device**
from data the official MyAnimeList API already returned. They are not sent anywhere.

Data stored by MyAnimeList itself is governed by MyAnimeList's own terms and privacy
policy.

## Data Sharing

We do not sell, rent, or share your personal information with third parties.

Network requests may be made to:

- **MyAnimeList**, including `myanimelist.net` and `api.myanimelist.net`, for official
  API access, OAuth authentication, web fallback pages, images, news (RSS), forum
  content, and community content.
- **AnimeSchedule** (`animeschedule.net`), used read-only and on-device, to determine
  which anime on your *Watching* list are currently airing for new-episode reminders.
- **YouTube** (`youtube-nocookie.com` / `img.youtube.com`), only when you tap a video
  embedded in a forum post or news article: the official YouTube IFrame embed is loaded
  in a WebView so the trailer/PV can play in-app. We never extract or proxy the video.
- **Optional metadata providers** used by the App, such as AniList, when enabled, to
  display supplementary read-only anime or manga metadata.
- Image, RSS, CDN, or media sources referenced by the content displayed in the App or
  inside fallback web pages.

Your use of MyAnimeList is governed by MyAnimeList's own Privacy Policy:

https://myanimelist.net/about/privacy_policy

If optional metadata providers, AnimeSchedule, or YouTube embeds are used, your use of
content from those services may also be subject to their own terms and privacy policies.

## Analytics and Advertising

The App contains **no third-party analytics, tracking, or advertising SDKs**.

If this ever changes, this Privacy Policy will be updated and, where required by law,
your consent will be requested first.

## Your Choices and Data Deletion

You can control locally stored data in the following ways:

- **Log out** from NakamaList to clear stored MyAnimeList API tokens from your device.
- **Log out** from MyAnimeList pages opened inside the WebView to clear your active
  MyAnimeList web session where applicable.
- **Clear app data** from Android system settings to remove locally stored app data,
  preferences, cache, tokens, and WebView-related local state.
- **Uninstall** the App to remove locally stored app data from your device.
- To manage data held by MyAnimeList itself, use your MyAnimeList account settings.

## Children's Privacy

NakamaList is intended for users who meet MyAnimeList's minimum age requirements.
The App is not directed to children who do not meet those requirements, and we do not
knowingly collect data from them.

## Permissions

The App requests only the Android permissions necessary for its features, such as:

- Internet access for API requests, images, news, and web fallback pages.
- Notification permission if you choose to enable notifications.
- Other permissions only if required by a feature you explicitly use.

## Security

NakamaList is designed to minimize sensitive data handling.

Security principles include:

- The App never stores your MyAnimeList password.
- The App does not operate a backend server for your personal data.
- Authentication tokens are stored locally using Android platform security features.
- Tokens and passwords are never logged.
- WebView fallback is used only as a user-facing browser surface, not as a scraping
  or data extraction layer.
- Unsupported MyAnimeList actions are performed only through user interaction with
  MyAnimeList-controlled pages.

## Open Source Software

NakamaList is built with open-source libraries. The full list of those libraries and
their licenses is available in the App under **Settings → App information → Open source
licenses**.

## Changes to This Policy

We may update this Privacy Policy as the App evolves. Material changes will be
reflected by updating the effective date above and, where appropriate, an in-app
notice.

## Contact

Questions about this Privacy Policy can be raised by email or through the project repository:

Email: nakamalist@proton.me

https://github.com/asa07-salihg/NakamaList