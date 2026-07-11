## 1.2.2
**swipe between seasons + always opens on this season**

- Swipe left or right on the Seasonal screen to move between Last, This Season, Next and the Archive - the same fluid tab transition My List got in 1.2.1. Neighbouring seasons preload as you swipe.
- The top bar follows the swipe too: the tab underline glides between tabs, and the filter/sort toolbar slides together with its season's content.
- My List's status-tab underline now glides with your swipe as well, instead of catching up after the page settles.
- Seasonal no longer stays wherever you left it: entering the tab always lands on the current season (jumping to a season from a detail page still works as before).

## 1.2.1
**Swipe between My List tabs + smoother sorting**

- Swipe left or right on My List to move between the status tabs (All, Watching, Completed, and so on).
- Changing the sort or its direction no longer flickers: the list now jumps straight to the top cleanly.

## 1.2.0
**Sort direction toggle + richer grid cards**

- Sort menus (My List, Seasonal, and studio/staff pages) now have an ascending/descending toggle next to them, defaulting to largest-first.
- My List grid cards now match the Home style: score chip top-left (tap for a quick score), an edit button bottom-left, and +1 bottom-right while watching. Grid vs rows now shows instantly with no flash when you open My List.

## 1.1.9
**Grid view for My List, and one Account section**

- My List has a new poster grid layout (Home-style cards with cover, progress, a tap-to-set score chip and a quick +1), switchable from a full-width toggle in Settings under My List.
- Settings now has a single "Account" section: MyAnimeList and AniList each get their own Sign in / Log out row instead of two separate sections.

## 1.1.8
**AniList profile, cleaner AniList-only experience**

- The Profile screen can now show your real AniList statistics (mean score, days, episodes, per-status counts, and manga stats), fetched straight from AniList.
- When both accounts are linked, a segmented toggle at the top of Profile switches between MyAnimeList and AniList instantly.
- With an AniList-only sign-in, MyAnimeList-only sections (News, Clubs, Forums and the Home history feed) are now hidden and locked, so nothing opens empty.
- Episode and list-news notifications now work from your AniList list too.
- Onboarding now asks you to connect your account right after the welcome, before the appearance and navigation preferences.
- Signed-out Profile, My List and Home no longer say "MyAnimeList" in their sign-in prompts, since you can now sign in with AniList too.
- "Open full profile" now opens AniList when you are viewing your AniList profile (and MyAnimeList for the MyAnimeList profile), instead of always opening MyAnimeList.

## 1.1.7
**Edit from AniList, and pick your profile source**

- With an AniList-only sign-in you can now edit your list: +1 progress, score, status, progress and removals write straight to AniList.
- When both MyAnimeList and AniList are linked, Settings has a new Profile source switch to choose which account backs your Profile screen.

## 1.1.6
**Use NakamaList with just AniList**

- You can now sign in with only your AniList account: your anime and manga list, Home rails and profile stats load straight from AniList, with no MyAnimeList account required. Editing your list from an AniList-only sign-in is coming in a follow-up.

## 1.1.5
**One place to sign in**

- Tapping Sign in anywhere in the app now opens a single connect screen that offers both MyAnimeList and AniList, instead of jumping straight into MyAnimeList.

## 1.1.4
**Discover starts at the top**

- Discover now opens pinned to the top, so the "Suggested for You" rail is fully visible instead of starting scrolled just past it.

## 1.1.3
**Consistent layout on every device**

- NakamaList now renders at a consistent default scale regardless of your system Font size and Display size (Screen zoom) settings, so the layout looks as designed and no longer shifts or clips on devices with those turned up.

## 1.1.2
**Clubs layout fix on large fonts**

- The Clubs cards now grow to fit their text instead of clipping it, so titles and subtitles stay fully visible when you use a larger system font size or display zoom.

## 1.1.1
**Your MyAnimeList history on Home**

- A new feed button at the top right of Home (matching the bell) switches between your personalized Home and MyAnimeList's four history feeds: Recent Anime, Recent Anime by Episode, Recent Manga, and Recent Manga by Chapter.
- History entries look like My List rows - poster, the full status in its color ("Completed 26/26 ep"), and the same score chip with the quick score menu. Tap the poster to open the title; tap the rest of the card to jump straight into that episode's or chapter's forum discussion in-app.
- Home now always starts at the top when you return to it, so New Episodes and Continue Watching can no longer stay hidden above the fold.
- Empty feeds say "no activity yet" instead of an error (your MyAnimeList list must be public for history feeds to work).

## 1.1.0
**Stability, sign-in reliability and translation fixes**

- Fixed the rare "randomly signed out" problem: a flaky connection or two requests refreshing your MyAnimeList session at the same time no longer log you out.
- Restoring the app to a new phone (device transfer / cloud backup) no longer risks a crash on first launch - you simply sign in again.
- The app language you pick now also works on Android 8-12 (it previously only applied on Android 13+), and notifications, forum spoiler buttons, chart titles, dates and many other texts now follow your chosen language.
- Tapping a notification while the app is closed opens reliably on every device.
- My List actions (+1, score, edit) can no longer touch the wrong entry when an anime and a manga share the same MAL id.
- The edit sheet now pre-fills your saved start/finish dates.
- Fixed several "old screen data flashes in" races (Forums back navigation, fast season switching, search Load more), smoother profile analytics and forum posts on large lists, and the genre chord chart draws with far less overhead.
- Sync no longer overwrites your exact AniList score when only status/progress differ, and failed AniList writes are now counted correctly.

## 1.0.30
**Score scales as a list**

- The score scale options are now stacked one per row (like a list), in Settings and onboarding, so they're easier to read and pick.

## 1.0.29
**Simpler score scales**

- Removed the 5-star scale and made the scale picker show every option at once (no more hidden, scrolled-off choices). Remaining scales: 100 Point, 10 Point Decimal, and 10 Point.

## 1.0.28
**Finer score sorting**

- Sorting My List by score now uses your exact score, so two titles with the same rounded 1-10 (e.g. 85 and 87) order correctly instead of tying.

## 1.0.27
**Whole 5-star scores**

- On the 5-star scale, scores now show as whole stars (each star = 2 points on the 10-point scale) instead of odd half-star values like 3.5.

## 1.0.26
**Scoring polish**

- Fixed the score bar looking broken on the 100-point scale (it now matches the clean episode bar), merged score scale and rounding into one Score setting with a single connected example, and renamed the scales to match AniList (100 Point, 10 Point Decimal, 10 Point, 5 Star).

## 1.0.25
**AniList-first scoring**

- With both MyAnimeList and AniList linked, you can now score in your chosen scale (100-point, 10-point decimal, or 5-star): the exact value is saved to AniList and a rounded 1-10 to MyAnimeList, and your fine score is read back from AniList so it sticks. The score picker follows your scale (and scrolls when it's long), and Settings shows a MAL/AniList example for each format.

## 1.0.24
**Final score prompt**

- Finishing a series with a quick +1 now pops up a small "Final score" card so you can rate it in one tap; back or the X dismisses it.

## 1.0.23
**Faster notifications**

- Background checks now run every 15 minutes instead of every few hours, so episode and news alerts arrive much sooner.

## 1.0.22
**More reliable background notifications**

- Background notification checks now wait for a network connection and re-arm themselves on launch, so new-episode and news alerts are more likely to arrive without opening the app. (If your phone still holds them back, exclude NakamaList from battery optimization in system settings.)

## 1.0.21
**Sort and filter studio & person works**

- Studio and character/staff pages now have a sort menu (Default, Score, Member, Air/Pub date) and a My List filter (Not in My List / In My List / Planned), so you can quickly narrow a person's or studio's works to what you haven't seen yet.

## 1.0.20
**Studios and authors open in-app**

- Tapping a studio now opens its works inside the app, and tapping a manga author opens their person page (the same one the cast uses) instead of jumping to the browser; both fall back to the web page if AniList has no match.

## 1.0.19
**Android 15 edge-to-edge cleanup**

- Dropped the deprecated status/navigation bar color attributes (ignored on Android 15); system bars are now transparent edge-to-edge and their icon contrast follows your selected theme.

## 1.0.18
**Live next-episode countdown**

- Currently-airing anime now show a live "Ep N: 45d 9h 40m" countdown to the next episode in place of the aired date, sourced from AniList; finished titles keep the date range.

## 1.0.17
**Episode notifications open the discussion**

- Tapping a new-episode notification (tray or bell) now jumps straight to that episode's in-app forum discussion, and works without leaving the bell.

## 1.0.16
**Notification fix**

- The new-episode bell feed and notifications now open the title in the app (with its episode discussions) instead of an external website.

## 1.0.15
**Notification fix**

- Tapping a new-episode notification now opens the title in the app (with its episode discussions) instead of a website.

## 1.0.14
**Full localization**

- The newest features are now translated into every supported language.

## 1.0.13
**Crash fix**

- Fixed a rare crash when leaving a detail page while its trailer or theme-song player was on screen.

## 1.0.12
**Adaptation links**

- The manga an anime is based on (and vice-versa) now shows under Related, sourced from AniList to fill the gap MyAnimeList's API leaves blank.

## 1.0.11
**Onboarding reorder polish**

- Reordering in first-launch setup now uses the exact same mechanism as Settings, with no scroll-vs-drag conflict.

## 1.0.10
**Score and setup polish**

- Score options sit on one row, the edit score shows in your chosen scale, score rounding explains each option, Sync settings appear only when both accounts are linked, and onboarding reorder drag is fixed.

## 1.0.9
**More of someone's works**

- People with lots of credits now have a "Load more" on their page instead of stopping at the first 50.

## 1.0.8
**Score scale in setup**

- You can now pick your score scale during first-launch setup, and drag-to-reorder works in both directions everywhere.

## 1.0.7
**Reorder fixes**

- Drag-to-reorder now works in both directions and is available in the first-launch setup too.

## 1.0.6
**Pick your score scale**

- You can now show your own scores on a different scale (100-point, decimals, 5 stars or 3 smileys) from Settings > Score.

## 1.0.5
**Drag to reorder**

- You can now long-press and drag a navigation row to reorder it, alongside the existing up/down arrows.

## 1.0.4
**Fullscreen and fuller credits**

- Trailers and theme songs can now go fullscreen, and people pages include their manga works alongside anime.

## 1.0.3
**Polish**

- Unrated rows in My List now match the rated style, and people pages show more of someone's works.

## 1.0.2
**Choose your start tab**

- You can now pick which tab opens when you launch the app: star it in Settings > Navigation.

## 1.0.1
**Sync and quality-of-life update**

- Adds a sync clean-up mode and score-rounding option, a quick score picker and score filter in My List, and fixes the notification-tap crash, edit-sheet touches, ranking order, and full-list sync.

## 1.0.0
**NakamaList 1.0**

- The first stable release: track your anime and manga, browse Discover and Seasonal, read News, Forums and Clubs, see your profile stats, get airing and news notifications, and optionally connect AniList.

## 0.17.8
**Localized UI**

- The UI is localized into 56 languages.

## 0.17.7
**Continue Reading widget**

- Added a home-screen Continue Reading widget.

## 0.17.6
**Continue Watching widget**

- Added a home-screen Continue Watching widget.

## 0.17.5
**Automatic AniList write-through**

- Once both accounts are linked, any change you make to your MyAnimeList list is mirrored to AniList automatically in the background.

## 0.17.4
**MyAnimeList to AniList sync**

- Added MyAnimeList to AniList list sync.

## 0.17.3
**AniList community reviews**

- Added optional AniList community reviews.

## 0.17.2
**List-news notifications**

- Added list-news notifications.

## 0.17.1
**Airing notifications**

- Added airing notifications.

## 0.17.0
**Clubs browser**

- Added a Clubs browser.

## 0.16.9
**Read-only Forums**

- Added read-only Forums.

## 0.16.8
**News**

- Added News.

## 0.16.7
**Seasonal**

- Added Seasonal.

## 0.16.6
**Rich manga detail pages**

- Added rich manga detail pages.

## 0.16.5
**Rich anime detail pages**

- Added rich anime detail pages.

## 0.16.4
**Discover**

- Added Discover.

## 0.16.3
**Personalized Home**

- Added a personalized Home.

## 0.16.2
**Full list management**

- Added full list management with read and write support.

## 0.16.1
**On-device analytics**

- Added on-device analytics.

## 0.16.0
**Profile statistics**

- Added your profile with full anime and manga statistics.

## 0.15.7
**Official sign-in**

- Added official sign-in.

## 0.15.6
**AniList sync write-through actions**

- Add, edit, +1 and remove actions on your MyAnimeList list are mirrored to AniList automatically in the background.

## 0.15.5
**AniList sync pacing**

- AniList sync requests are paced at about 25 requests a minute to stay comfortably within AniList's rate limit.

## 0.15.4
**AniList sync progress notification**

- The sync runs in the background with a progress notification, so you can leave the screen while it works.

## 0.15.3
**AniList score conversion**

- Scores are converted between AniList's 100-point scale and MyAnimeList's 1-10 scale.

## 0.15.2
**One-way AniList list copy**

- The Sync with AniList screen lets you copy status, progress and score one way, either MyAnimeList to AniList or AniList to MyAnimeList.

## 0.15.1
**AniList list comparison**

- The Sync with AniList screen compares your two lists by matched title and shows the titles that differ.

## 0.15.0
**Sync with AniList**

- If you sign in to both MyAnimeList and AniList, a new Sync with AniList screen is available in Settings.

## 0.14.5
**AniList account settings**

- Settings now manage your AniList account under its own header.

## 0.14.4
**MyAnimeList account settings**

- Settings now manage your MyAnimeList account under its own header.

## 0.14.3
**Optional AniList setup sign-in**

- The first-launch welcome can optionally guide you through signing in with AniList.

## 0.14.2
**MyAnimeList setup sign-in**

- The first-launch welcome can guide you through signing in with MyAnimeList.

## 0.14.1
**Replay welcome**

- The welcome flow can be replayed anytime from Settings.

## 0.14.0
**Welcome aboard**

- Added a skippable first-launch welcome that walks you through setup and then drops you on Home.

## 0.13.7
**Widget +1 action**

- Continue widgets now let you tap "+1" to advance the episode or chapter right from the widget.

## 0.13.6
**Widget edit shortcut**

- Continue widgets now let you tap the pencil to jump straight to the edit sheet.

## 0.13.5
**Widget title opening**

- Tapping a title in a Continue widget opens it in the app.

## 0.13.4
**Widget navigation arrows**

- Continue widgets now have left and right arrows to flip through your in-progress titles.

## 0.13.3
**Widget poster card**

- Continue widgets now show a full poster card.

## 0.13.2
**Continue Reading widget**

- Added a Continue Reading home-screen widget that mirrors your Home rail.

## 0.13.1
**Continue Watching widget**

- Added a Continue Watching home-screen widget that mirrors your Home rail.

## 0.13.0
**Continue widgets**

- Added home-screen Continue widgets.

## 0.12.4
**Review score display**

- AniList review scores are shown on the familiar 1-10 scale.

## 0.12.3
**Full review reader**

- Tapping a review opens it in full inside the app.

## 0.12.2
**More AniList reviews**

- A "Show more" option opens the full AniList review list on a title's detail page.

## 0.12.1
**AniList reviews on detail pages**

- Community reviews sourced from AniList are now shown on a title's detail page.

## 0.12.0
**AniList account**

- You can optionally sign in with AniList from Settings.

## 0.11.4
**Manual update checks**

- Added "Check for updates now" to check for new episodes and news on demand.

## 0.11.3
**Cache storage control**

- You can view and clear the app's cached data from Settings.

## 0.11.2
**Surprise me**

- Added a dice button on Discover that opens a random top anime.

## 0.11.1
**Share titles**

- You can share any anime or manga to other apps from its detail page.

## 0.11.0
**Storage and discovery tools**

- Added share, surprise me, storage control and manual update tools.

## 0.10.5
**Top Ranked Manga**

- Added Top Ranked Manga to Discover.

## 0.10.4
**Top Ranked Anime**

- Added Top Ranked Anime to Discover.

## 0.10.3
**Discover rank badges**

- Ranked Discover lists show titles by their MyAnimeList rank with a #rank badge in the full view.

## 0.10.2
**Load more search results**

- Search results now have a Load more button that fetches the next page instead of stopping at the first batch.

## 0.10.1
**More detail-page lists**

- Related and Recommendations now have a "Show more" link that opens the full list as a top-to-bottom card view.

## 0.10.0
**Explore more in Discover**

- Every Discover row now has a "Show more" link that opens the full list as a top-to-bottom card view with a Load more button.

## 0.9.23
**Right-to-left language support**

- Added right-to-left support for Arabic, Hebrew, Persian and Urdu.

## 0.9.22
**56 languages**

- The whole app is now translated into all 56 languages offered in the language picker.

## 0.9.21
**Language picker**

- You can pick your language in Settings -> Language.

## 0.9.20
**Live News Discussion lookup**

- The in-app news reader now checks the live News Discussion board when looking for a brand-new article's full text.

## 0.9.19
**Forum search news fallback**

- The in-app news reader still uses forum search as part of finding the full article body.

## 0.9.18
**Filtered person-page entries**

- Person pages now list only anime that exist on MyAnimeList.

## 0.9.17
**Person-page 404 prevention**

- Tapping an entry on a person page no longer opens a 404.

## 0.9.16
**Filtered unmatched person entries**

- Manga and unmatched entries are filtered out on person pages.

## 0.9.15
**Buy me a coffee**

- Added a "Buy me a coffee" button at the bottom of Settings so you can support development if you'd like.

## 0.9.14
**What's New title cleanup**

- Tidied the What's New screen, which was showing its title twice.

## 0.9.13
**Character anime appearances**

- A character's page now lists the anime they appear in.

## 0.9.12
**Character appearance roles**

- Character appearance entries now show the character's role.

## 0.9.11
**Tappable character appearances**

- Each character appearance entry is tappable and opens that anime.

## 0.9.10
**Cast and staff label clipping fix**

- Fixed a corner-clipping glitch on the bottom label of cast and staff cards.

## 0.9.9
**Your language**

- Added support for choosing your language from Settings.

## 0.9.8
**More reliable news**

- The in-app news reader now finds a brand-new article's full text more reliably.

## 0.9.7
**Fewer broken links**

- Person pages now avoid entries that would open broken MyAnimeList links.

## 0.9.6
**Support the app**

- Added an optional way to support development from Settings.

## 0.9.5
**Character appearances**

- Character pages now include anime appearance information.

## 0.9.4
**Roles on person pages**

- Person pages now list anime roles for voice actors and staff members.

## 0.9.3
**Character and staff pages**

- Tap any character, voice actor or staff member to open their page with full image and bio from AniList.

## 0.9.2
**Staff**

- Added a swipeable Staff rail above Theme Songs, with the complete list behind "More staff".

## 0.9.1
**Characters and voice actors**

- Added a swipeable Characters rail, each paired with its Japanese voice actor, with the complete cast behind "More characters".

## 0.9.0
**Trailers**

- The official trailer, or PV, now plays inline on the anime detail page between the synopsis and the info grid.

## 0.8.7
**In-app theme song playback**

- Theme song videos now play in-app, with no browser required.

## 0.8.6
**Ending themes**

- Ending themes are now available on the anime detail page.

## 0.8.5
**Opening themes**

- Opening themes are now available on the anime detail page.

## 0.8.4
**AnimeThemes source**

- Anime detail page theme songs are sourced from AnimeThemes.

## 0.8.3
**Theme song playback**

- Theme songs now play inline in swipeable Openings and Endings pagers.

## 0.8.2
**What's New**

- Added the What's New screen on the Version row.

## 0.8.1
**Clear WebView data**

- Added a working "Clear WebView data" action in Settings.

## 0.8.0
**Customizable navigation**

- You can now show, hide and reorder bottom-navigation destinations.

## 0.7.12
**Classic navigation layout**

- The classic bar spreads tabs evenly when there are five or fewer.

## 0.7.11
**Pinned Settings tab**

- Settings stays pinned in the customizable navigation.

## 0.7.10
**Genre Connections filters**

- Added list-status, min-score and node-count filters to Genre Connections.

## 0.7.9
**Genre Connections tabs**

- Added Genres, Themes and Demographics tabs to Genre Connections.

## 0.7.8
**Genre Connections chord**

- The Genre Connections graphic was rebuilt as a real woven chord.

## 0.7.7
**Type and format analytics**

- Added a type/format breakdown to profile analytics.

## 0.7.6
**List-by-genre analytics**

- Added list-by-genre analytics, with genre counts that open My List filtered to that genre.

## 0.7.5
**Score distribution analytics**

- Added score distribution to profile analytics.

## 0.7.4
**Profile analytics**

- Added on-device, MyAnimeList-style analytics.

## 0.7.3
**Licenses and legal**

- Added an open-source licenses screen.

## 0.7.2
**Clubs**

- Added a Clubs tab with name search and a category filter that opens the matching MyAnimeList page.

## 0.7.1
**Performance pass**

- Added one shared network client app-wide.

## 0.7.0
**Richer forum posts**

- Forum posts now support full MyAnimeList BBCode.

## 0.6.8
**Inline YouTube in forum posts**

- Added inline YouTube playback in forum posts.

## 0.6.7
**Animated GIFs in forum posts**

- Added animated GIF support in forum posts.

## 0.6.6
**Forum post formatting**

- Forum posts now support quotes, spoilers, code, tables, alignment and sizes.

## 0.6.5
**In-place discussions**

- Episode and chapter discussions open in place.

## 0.6.4
**Matched forum discussions**

- Discussion threads on detail pages are matched from the forums.

## 0.6.3
**Episode and chapter discussions**

- Added episode and chapter discussion threads on the detail page.

## 0.6.2
**In-app news reader**

- Added a reader that recovers the full article body from its forum topic.

## 0.6.1
**Forum reading**

- Added read-only Forums with boards, topics and posts.

## 0.6.0
**Detail polish**

- Added a single centered poster carousel.

## 0.5.8
**Seasonal detail jump**

- Added a tap-to-open Seasonal jump on the detail page.

## 0.5.7
**Collapsible background**

- Added a collapsible background on the detail page.

## 0.5.6
**Two-column info grid**

- Added a two-column info grid on the detail page.

## 0.5.5
**Status-distribution bars**

- Added real status-distribution bars on the detail page.

## 0.5.4
**In-app recommendation back-stack**

- Tapping a related or recommended title pushes it onto an in-app back-stack.

## 0.5.3
**Recommendations rail**

- Added Recommendations poster rails on the detail page.

## 0.5.2
**Related rail**

- Added Related poster rails on the detail page.

## 0.5.1
**Related and recommendations**

- Added Related and Recommendation poster rails on the detail page.

## 0.5.0
**Detail screen**

- Added a full anime and manga detail overlay openable from any screen.

## 0.4.5
**Floating edit/add button**

- Added a list-synced floating edit / add button on the detail overlay.

## 0.4.4
**Seasonal add action**

- Seasonal cards now support add.

## 0.4.3
**Seasonal plus-one action**

- Seasonal cards now support plus-one.

## 0.4.2
**Settings persistence**

- Every preference now survives a cold start and is saved on-device.

## 0.4.1
**Seasonal cards**

- Added list-aware Seasonal cards with quick edit.

## 0.4.0
**Home**

- Added a real Home screen.

## 0.3.10
**This Season rail**

- Home includes This Season.

## 0.3.9
**Plan to Watch/Read rail**

- Home includes Plan to Watch/Read.

## 0.3.8
**New Episodes rail**

- Home includes New Episodes.

## 0.3.7
**Continue Reading rail**

- Home includes Continue Reading.

## 0.3.6
**Continue Watching rail**

- Home includes Continue Watching.

## 0.3.5
**List actions in search results**

- List actions are available directly on search results.

## 0.3.4
**Search suggestions**

- Search includes suggestions.

## 0.3.3
**Discover search**

- Added full-screen search with recents and content filtering.

## 0.3.2
**Discover rails**

- Added live ranking rails for top, airing, upcoming and more.

## 0.3.1
**Editing your list**

- Added a full edit sheet that writes back to MyAnimeList, with optimistic updates that apply instantly while syncing.

## 0.3.0
**My List**

- Added a live My List.

## 0.2.8
**Airing badges**

- My List includes airing badges.

## 0.2.7
**My List sorting**

- My List includes sorts.

## 0.2.6
**My List type filters**

- My List includes type filters.

## 0.2.5
**My List status tabs**

- My List includes status tabs.

## 0.2.4
**Bell feed**

- Added a bookmarkable bell feed.

## 0.2.3
**Local notifications**

- Added local notifications.

## 0.2.2
**Notifications**

- Added notifications.

## 0.2.1
**Your profile**

- Added a real profile with full anime and manga statistics.

## 0.2.0
**Sign in**

- Added MyAnimeList sign-in via the official OAuth flow.

## 0.1.8
**On-device cache**

- Added a compliant on-device cache for faster, offline-friendly reads.

## 0.1.7
**Browser fallback**

- Added a selectable browser fallback.

## 0.1.6
**Per-app language**

- Added per-app language.

## 0.1.5
**Theme modes**

- Added theme modes: System, Light and Dark.

## 0.1.4
**Theme and language**

- Added theme and language settings.

## 0.1.3
**News**

- Added MyAnimeList news via the official RSS feed.

## 0.1.2
**Seasonal**

- Added a live Seasonal browser with an archive back to the earliest seasons.

## 0.1.1
**Identity**

- Added a distinct violet identity with a user-selectable accent palette.

## 0.1.0
**Foundations**

- Added the MyAnimeList-first app shell with the swipe "revolver" navigation.
