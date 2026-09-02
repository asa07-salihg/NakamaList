## 1.7.4
**Recent Activity stops waiting on a title's page**

- Your friends' scores and their artwork now appear on Recent Activity the first time you open it. They come from your friends' lists, and until now only a title's page ever went and got those - so the rows were bare unless you happened to open something first, and looked fixed once you came back. Recent Activity fetches them itself now.
- They arrive as each friend's list lands rather than all at the end, and the feed itself is not held up waiting for them. A list saved from a previous run shows straight away.

## 1.7.3
**Two episodes in one minute**

- Recent Activity could close the app while showing your own history. MyAnimeList records the time only down to the minute, so marking two episodes of the same show inside one minute arrived as two entries that looked identical in every way, and the list could not show both. It tells them apart by episode now.
- Your friends' activity, News and the Discover rows read their feeds the same way, so they were open to the same thing. An entry that arrives twice is shown once now, rather than being left to close the app.

## 1.7.2
**Friend Scores, in one place and kept properly**

- A title's page is ordered properly now. Everything about the title comes first, then everything about people, in one run: Discussions, then Status distribution, then Friend Scores.
- The friends' chart had its own "Score Distribution" heading up beside Status distribution, which read as the site's scores rather than your friends'. It has moved into Friend Scores, under the cards - one section, one heading, and whose scores it is says so.
- Every friend who has the title now appears, including Plan to Watch and anyone who has not rated it. Their card shows how far in they are with an empty score. The average and the chart still count only the people who actually gave a score, so the numbers are unchanged.
- The Friends page opens on whichever of Friend Lists and Recent Activity you were last on, and remembers it between launches. It used to snap back to Friend Lists every time you stepped away to a title, which meant re-picking Recent Activity on every return.
- Only that choice is remembered. Coming back puts you at the top of that segment - not inside a friend's open list, not on a feed filtered to one person, and not halfway down your friends where you had scrolled to. It is simply there when the screen appears, with none of the sliding-back-into-place you could watch happen.
- Recent Activity rows show the artwork more often. A friend watching something you have never touched used to draw a grey question mark on the MyAnimeList side; the poster now comes from that friend's own list, which the app already has.
- Your friends are listed alphabetically. They used to appear in the order you added them, which stops being findable somewhere around the tenth name - and the AniList side was already sorted by name, so the same screen was ordered two different ways depending on which account you were on.
- Friends' lists are stored properly on the device now instead of being kept only in memory. They used to be thrown away every time the app closed, so the first title you opened after a restart had to fetch every friend again. They survive now, and the week-old refresh rule finally means a week.

## 1.7.1
**Two things the release checks caught**

- Both halves of adding a friend now report problems the same way. The MyAnimeList side was passing text identifiers around inside the data layer, which the build tooling flagged as meaningless; it answers with a result the screen turns into words, exactly as the AniList side already did.
- No change you can see. This one is housekeeping so the release build passes its own checks.

## 1.7.0
**A dial for your color**

- The color picker is a dial now, with a hand that swings to the one you pick. The white ring around the chosen swatch is gone - a white circle on a page about color read as a scratch, not as a highlight.
- Fixed: choosing Grid in setup left the example above showing a row. It shows real grid cells now.
- If you skip signing in, the example row is Fullmetal Alchemist: Brotherhood rather than a blank placeholder, so you can see what a filled row actually looks like.

## 1.6.9
**The star, and some light**

- The bottom bar page in setup was missing the star that picks which tab opens when you launch the app. Settings had it, setup didn't, and it was the same list of rows in both. Now they match.
- Every setup page carries a soft wash of your accent colour behind it, so picking a colour shows up everywhere rather than only on the page that asks.

## 1.6.8
**A first run worth having**

- Setting up NakamaList used to be three screens, the last of which stacked nine settings into one long scroll. It is now one thing per page, and every page shows you what it is talking about. Tap a theme and the screen repaints. Pick a colour and it runs through everything. Choose a layout, a score scale or a title language and a real list row redraws in front of you.
- Once you have signed in, that row is your own series at your own episode, not a mock-up.
- Nothing was taken away. The navigation order, adult titles and notifications each got a page of their own instead of a switch in a pile.
- Swipe between pages, or use the button. A thin bar shows how far along you are.

## 1.6.7
**Five tabs that fit in every language**

- Fixed: the Recent Activity tabs were sized for English. In several languages the longest word did not fit its fifth of the screen and was cut short - "Afleveringen" arriving as "Afleveringe...". The strip now sizes itself to the longest label it was given.

## 1.6.6
**Export and Import, said plainly**

- The two friends backup rows are called Export and Import now, and carry an arrow out and an arrow in rather than the chevron every other row uses. The chevron promises a screen on the other side; these two hand off to the file picker and come straight back.

## 1.6.5
**Your friends list can be saved now**

- Settings has a Friends section, under My List: save your friends to a file, and load one back. Moving to a new phone, or reinstalling, no longer means typing every name again.
- Loading merges rather than replaces, so restoring a backup onto a phone that already has friends on it leaves you with both.
- It will also read a plain list of usernames, one per line, so you can paste names in from anywhere instead of adding them one at a time.
- This covers the MyAnimeList names only, and the note in Settings says so: they live on your device and nowhere else, which is exactly why they can be lost. Who you follow on AniList is on your AniList account and comes back when you sign in.

## 1.6.4
**Swipe between your friends' activity feeds**

- The filter menu on Recent Activity is gone. The categories are pages you swipe between, with the same strip the home page uses, so getting from All to Chapters is a drag rather than a menu.
- Each category keeps its own place in the list, and changing person or search takes you back to the top.

## 1.6.3
**The same five on your friends' activity**

- Your friends' Recent Activity has the same filter the home page got: All, Anime, Episodes, Manga, Chapters. As on the home page, All shows the list updates and the per-episode detail sits one option across.
- The AniList side keeps All, Anime and Manga, because AniList publishes one activity stream rather than four feeds. There is no list-update-versus-episode distinction there to offer, and two options that could only ever be empty would be worse than not having them.

## 1.6.2
**All four of your history feeds**

- Recent Activity has five tabs again: All, Anime, Episodes, Manga, Chapters. MyAnimeList publishes four history feeds and only two were being read, so the per-episode and per-chapter ones had nowhere to appear.
- All still shows the list feeds only. The episode feed restates the same events one episode at a time, so putting everything in one tab meant two rows saying the same thing about the same title at the same second. The finer view is one tab across.

## 1.6.1
**Scrolling on Recent Activity**

- Fixed: scrolling Recent Activity on the home page stuck, jumped or refused to move. Every category was sharing one scroll position, and while a swipe was in flight two lists of different lengths were writing into it at once. Each category keeps its own place now.

## 1.6.0
**Following people from here**

- You can now follow and unfollow AniList accounts from the Friends page, the same way you add and remove MyAnimeList names. The form and the list work identically; only the words differ, because these two are not the same act. A MyAnimeList name is a note kept inside this app, since MyAnimeList has no way to share a friends list. Following on AniList is real: it happens on your account, and the person can see it.
- The buttons say so. Add and Remove on the MyAnimeList side, Follow and Unfollow on the AniList side.
- Fixed: signing in as a different AniList account showed the previous account's following list, and could load the previous account's list as your own. What the app remembered about a signed-out account is now dropped, including two things that had never been cleared by anything.

## 1.5.9
**Both sets of friends, and lists that do not sit still for a month**

- A title's page now shows your MyAnimeList friends and the people you follow on AniList at the same time, under a heading each. It used to show only whichever side the Friends page was set to, so half your friends were missing from a question that has one answer.
- A friend's list is pulled again once it is a week old. It was loaded once and believed for as long as the app stayed open, which is right for an afternoon and wrong for a month: somebody three episodes in when you last looked has probably finished since.
- Two people who use the same name on the two sites are two people now. They were one, and the second list loaded quietly replaced the first.
- Who you follow on AniList is worked out once every half hour instead of on every title you open. Pulling to refresh the Friends page still asks properly, so somebody you followed a minute ago shows up.
- A title's page only shows people who are still your friends. Unlinking AniList, or removing someone on the website, used to leave their score sitting there under a name that was no longer on any of your lists.
- Signing out of AniList now clears what was loaded about that account. It kept the previous account's follow list, so signing in as somebody else showed the wrong people. Your MyAnimeList friends are left alone.
- Opening Friends and going straight to Recent Activity could leave the feed empty until you pulled to refresh. It now waits for the list of people before fetching.

## 1.5.8
**Editing in bursts**

- Every quick +1 was reading your entire saved list back off storage before writing it out again. Watching four episodes in a row did that four times over. The list is now held once and edited in place, so a burst of edits costs one read instead of one each.

## 1.5.7
**Five things an audit turned up**

- Fixed: signing out left everything the app had loaded about other people in memory. Signing in as somebody else could show the previous account's friends' scores on a title's page.
- Fixed: removing someone left their score on every title's page. The Friends page said they were gone and the detail page disagreed. Their open list closes too.
- Fixed: two searches over friends' cached lists ran on the drawing thread - one when the activity feed landed, one every time a title's page opened. On a large friends list that was a visible stutter at exactly the wrong moment.
- Fixed: the friends' score chart put an AniList 85 in the 8 row while your Profile counted the same entry as a 9. Both round now.
- Fixed: moving between Home, Friends and Profile could leave the control in the top bar blank, when the screen you left cleared the slot after the screen you arrived at had filled it.

## 1.5.6
**The grid, and lists that keep up**

- A friend's list follows your own layout setting. If you read My List as a poster grid, theirs is a poster grid too. It had been rows either way, which made "the same screen" not quite true.
- Reading your friends' activity now also brings their lists up to date, without a single extra request. The feed already says who moved which title how far, so the cached lists take the change instead of waiting to be reloaded.
- Scores are the exception: neither MyAnimeList nor AniList sends a score with an activity update, so a friend's score still comes from the last time their list was loaded.

## 1.5.5
**Smoother on a long feed**

- Your friends' activity scrolls smoothly on a large list. Each row had been searching your whole list for its poster and a friend's whole list for their score, every time the screen redrew; both are now looked up directly.

## 1.5.4
**The bar holds what stays put**

- The MyAnimeList/AniList switch and the person picker swapped places on the Friends page: the account moved up into the top bar, the person came down to the control row. The account is chosen once a session and the person changes constantly, and the bar is where the eye goes for the answer that stays put.
- Profile's account switch moved to the same place, so it is the one control in the one spot across both pages. It used to take a row off the top of every screenful and scroll away with the page.
- Searching people from Recent Activity now shows the people. It used to open a field over the unchanged feed, with nothing on screen answering what you were typing; picking a name narrows the feed and closes the search.
- Fixed: the link to a title's score distribution on MyAnimeList went to a 404. The address was being built with the template text left in it rather than the title's number.
- Friend scores on a title's page are cards now, the same card the Friends page uses for people, with the score where the remove cross sits there. Each one also says how far that person got, in the status colour used everywhere else, so "green, near the end" reads before any of the words do. An 8 at three episodes and an 8 at the end are not the same claim.
- The friends' score distribution sits under Status distribution now, the exact chart your Profile draws. That block already answers "how did everyone receive this"; how many are watching it and what the people you know made of it are the same question.
- Loading a friend's list downloads noticeably less. It had been asking for everything your own list needs - tags, comments, priority, rewatch counts, your own dates, genres - none of which a read-only view of somebody else's list ever shows.
- The link to the full distribution moved into More on MyAnimeList, with the other ways out of the page.
- A friend's AniList list no longer says UNKNOWN on every row. The type, the season and the episode count were never asked for, though AniList has all three; the MyAnimeList side of the same screen had been complete all along.
- Pull to refresh now works from an empty feed and from a failed load - the two places you most want it. The message said to pull down and there was nothing to pull, because a line of text is not something you can drag.
- Swiping sideways no longer switches between Friend Lists and Recent Activity. That is what the icon on the left is for, and Friend Lists is itself a row of swipeable status tabs, so the gesture had two meanings. My List keeps its swipe, where it only ever means one thing.

## 1.5.3
**Find the right friend**

- Two searches, and neither can be mistaken for the other. The magnifier in the top bar searches **people** - that bar is about who you are looking at - and it is there on both views. The magnifier on the control row searches **what that view is showing**, so Recent Activity can now be searched by title.
- Both work exactly like My List's: the field takes over the row, and back closes it and clears what you typed.
- The name in the top bar gained a cross on its left when somebody is picked, so getting back to everyone no longer means opening the menu to find the entry that means "never mind". Both icons are the bell's size and sit against the name at whatever width it happens to be, so a long username shortens rather than pushing them off the bar.
- The "add someone" box hides itself while you are searching. A form asking for a new name is noise on a screen whose job at that moment is finding an existing one.
- Searching and finding nobody says so, rather than showing the "you have no friends yet" explanation to somebody who has plenty.

## 1.5.2
**A glyph instead of a code**

- The Friend Lists / Recent Activity switch is an icon now: My List's own list mark and the history mark Discover already uses. Tap it to see both names written out.

## 1.5.1
**Whose score is that**

- Fixed: a friend's activity row showed your score next to their name. Neither feed carries a score, so it now comes from their list once that has been loaded and stays blank until then. Blank is honest; your own number under someone else's name was not.

## 1.5.0
**Two views, one row**

- The Friends page lost a whole row of chrome. The tab strip is gone; which view you are on is now a name on the left of the same row that carries the account switch and the filter.
- My Friends folded into Friend Lists. It was a list of names you tapped to open a list, and Friend Lists already opened with that same list of names, so it was the same screen twice with a swipe between them. Adding and removing people now happens where the people are.
- Two views instead of three also means swiping left and right is a single step rather than a hunt.
- Removing someone stays on the MyAnimeList side, where the list is one the app keeps for you. Names on the AniList side come from your account's own follows, and unfollowing is a real action on your account, so there is no X there until that is built properly.

## 1.4.9
**A friend's list is your list**

- Reading a friend's list now happens on My List's own screen: the same status tabs, the same toolbar (anime/manga, type, sort, direction, search) and the same rows. Not a smaller lookalike of it, the screen itself. The only difference is whose list it is, and that is the picker in the top bar.
- It is read-only, so the edit and +1 buttons are gone rather than greyed out. They write to your list, and your list is not what is on screen.
- Titles with no artwork now show a "?" instead of an empty frame. MyAnimeList's activity feed carries no images at all, so a friend watching something you do not have had nothing to show; the mark says "no picture" rather than looking like a failed load. Rows from AniList still fill in on their own.

## 1.4.8
**One shape for choosing a view**

- Choosing between Home and Recent Activity moved into the top bar. It is a choice you make once, so it no longer takes a row of the page.
- The swipeable strip now belongs to Recent Activity and carries its categories, so All, Anime and Manga are pages you swipe between. Both feeds are fetched once and filtered on the device, so a swipe lands on a page that already has its content instead of emptying the list and going back to the network.
- Your friends' activity now uses the exact rows Home uses, not a lookalike: the poster, the progress bar, the full status line, and your own score on anything you also have.
- Picking a friend moved up to the top bar and starts on All, staying in the same place whether you are reading their activity or their list.
- The filter moved onto the MyAnimeList/AniList row, pinned right, which is exactly where My List keeps its own. It had been sitting on a strip of its own inside the page, so two halves of one question were on two different rows.
- Filter rows are centred throughout, which mattered most on tablets and televisions where they had been sitting against the left edge with a wide empty band beside them.
- Friends lists return to the top when you change a filter or switch person, the way My List already did.
- Friend scores on a title's page now fill themselves in, and appear one by one as each list arrives. There is no longer a button to press first.
- Fixed: opening a friend's list on AniList failed and blamed their privacy settings. The list was never private; the app had forgotten which account the name belonged to. It now remembers, and can look a name up when it does not.
- Fixed: Home came back where you left it instead of at the top, which pushed New Episodes off the screen on opening.

## 1.4.7
**What your friends thought**

- A Friend Scores block on every title's page: what each person on your Friends list gave it, your own score alongside theirs, and their average. Tap a name to open that person's list.
- It uses lists you have already opened, so it costs nothing. If some are missing it says how many and offers to fetch them once; after that every title you open is instant.
- A link straight to the full score distribution on MyAnimeList, for the picture across everyone rather than just your friends.
- Your own score is marked and left out of the friends' average, because an average that includes you is not one you can compare yourself against.

## 1.4.6
**A simpler Home**

- Home now has two buttons at the top instead of a hidden menu of five feeds: Home, and Recent Activity. Your own recent anime and manga updates arrive together in one list, newest first, with Anime and Manga filters.
- The old menu made you choose between "Recent Anime" and "Recent Anime by Episode", which were the same events described twice. One list, no choice to make.
- Pull down to refresh, on both views. On Home that reloads your list and rebuilds every rail; on Recent Activity it re-reads your feed instead of redrawing what was already cached.

## 1.4.5
**Read your friends' lists**

- The Friend Lists tab is live. Pick someone and browse what they are watching and reading, laid out like your own list, with their status, their progress and their score. Tap a title to open it.
- Filter by anime or manga and by status, exactly as you would your own list. Pull down to reload theirs.
- Nothing is editable there, because it is their list. Your own controls are on the title's page, one tap away.
- Fixed: with both accounts linked, switching to AniList still showed the MyAnimeList names you had typed. It now shows who you actually follow on AniList, and switching back returns your own list of names.

## 1.4.4
**What your friends are watching**

- The Recent Activity tab is live. Everyone on your Friends list, merged into one feed, newest first, with what they watched or read and how far along they are. Tap a row to open the title.
- Filter by anime or manga, or tap someone's name to see only them. Tap it again to go back to everyone.
- It loads when you open the tab and refreshes when you pull down, not on every visit. On the MyAnimeList side each refresh is a couple of requests per person, so it waits until you ask.
- A friend whose account has gone or whose list has been made private simply drops out of the feed instead of breaking it for everyone else.
- Status colours are now identical everywhere in the app. The edit sheet had quietly drifted to a darker grey for Plan to Watch.

## 1.4.3
**Friends**

- A new Friends tab. Add people by their MyAnimeList username and they stay on your list, ready for what comes next: their recent activity and their lists, both arriving in the following updates.
- If you also use AniList, a switch at the top lets you choose which account the page follows. Everyone you follow on AniList appears there on its own, with nothing to add by hand.
- MyAnimeList keeps friend lists to its own website, so they cannot be brought over automatically. The page says so plainly the first time you open it, rather than leaving you wondering.
- Names are checked as you add them, so a typo or an account with a private list is caught immediately instead of turning into an empty feed later.

## 1.4.2
**Every change, everywhere, at once**

- An edit made anywhere now appears everywhere immediately. Set a title to Watching from its page and it is on Home and in your list before you get back to them; a +1 from a Discover result updates the same title on Seasonal. Nothing waits for the server any more, and if a change is rejected it is undone rather than left on screen.
- Titles added to Plan to Watch or Plan to Read from another screen now show up on Home. They only appeared after a restart before.
- Episode counts can no longer read past the end of a series. Where MyAnimeList had you at 24 of 12 episodes, NakamaList shows 12 / 12, the same as the website. Your list on MyAnimeList is left exactly as it is.
- Pull to refresh on a title's page, like everywhere else. It refetches the page and your list entry rather than redrawing what was already cached.
- A Release Years chart in your profile statistics, showing how your anime list spreads across the years, right back to the oldest thing on it. Tap any year to open your list filtered to it. Thanks to the reader who wrote in asking for this.
- Films, OVAs and older anime now have a release year. MyAnimeList only tells apps the season for titles that belong to a broadcast season, so everything else was arriving with no year at all: missing from the new chart, and sorted to the bottom whenever you ordered your list by air date.

## 1.4.1
**Tablets, and a TV that actually works with a remote**

- Tablets are properly supported. The app rotates and fills the screen instead of sitting in a portrait strip with black bars, and grids and tab strips adapt to the width you actually have. Phones stay portrait, as before.
- Signing in works on TV. Sign-in now opens inside NakamaList rather than handing off to a TV browser, which usually opened on its own home page and lost the page it was asked for. It works from the welcome screen too, and closes itself once you are signed in.
- Press OK on a title to step into it, and its own buttons light up: the title itself, its score, edit, and +1. Move along them with left and right, press OK again to use one, and press back to step out. Every button on a card is reachable with the remote now.
- Left and right on the remote spin the revolver bar straight to the next tab. With the classic bar you move along the tabs and press OK, as you would expect.
- The selection outline is drawn to fit the thing it marks, instead of being cut off at the edge of a row or wrapped around a poster and its title together.
- The app now fills the whole TV screen. The safe-area margin added in 1.4.0 turned out to shrink it into a bordered box on sets that do not crop the picture, which is all of them.
- Posters and grids keep a sensible size on a big screen rather than being blown up, and the tab strips sit across the screen instead of bunching in one corner.
- The refresh button on TV is gone. It floated over the first row and added a stop to the remote's path for something the app already does on its own; pull to refresh is unchanged on phones and tablets.
- A new TV banner, matching the store artwork.

## 1.4.0
**NakamaList on the big screen**

- NakamaList now installs and runs on Android TV and Google TV. It appears in the TV launcher with its own banner, and the whole app is available - no cut-down version.
- Everything is usable with the remote: the D-pad moves between posters, rows and tabs, and whatever is selected is outlined in your accent colour so you can always see where you are.
- The app fills the screen properly on TV instead of being squeezed into a phone-shaped strip, and stays inside the safe area so nothing is cut off by the edges of your screen.
- Where you would pull to refresh on a phone, TV shows a refresh button you can reach with the remote.

## 1.3.9
**The right discussion thread, every time**

- Discussions on a detail page now show MyAnimeList's own thread for movies, OVAs, ONAs and specials, instead of an unrelated forum post that happened to share the title.
- Series that MyAnimeList files under a year, like "Suzumiya Haruhi no Yuuutsu (2009)", now find their episode discussions too: the forum names those threads with a season number instead of the year.
- The back button now closes the edit sheet when you open it from a Home rail, like it already did everywhere else.

## 1.3.8
**Pull to refresh, and a profile that keeps up**

- Pull down from the top of My List, News or Profile to refresh right away, with the standard Android indicator.
- Your profile statistics no longer lag behind: the entry counts, totals and mean score are now read from your own list, so they change the moment you edit an entry.
- Watched episodes update instantly too. A +1 is counted straight away, and the number is corrected the next time MyAnimeList publishes its own figure.
- The profile also refreshes itself when you edit something anywhere else in the app, instead of waiting for a restart.

## 1.3.7
**Sync progress that adds up**

- The count on the Sync screen and the one in the notification now always match. They are fed from the same place, and both switch to the real total at the same moment once the lists have been re-read.
- When a sync finishes, the progress notification is cleared, so you no longer see a finished run and a running one side by side with different numbers.
- Reopening the app mid-sync no longer resets the notification to a blank progress bar.

## 1.3.6
**Search inside your list**

- New search in My List: tap the magnifier next to the sort icon and the toolbar turns into a search bar. Type any title (romaji or English) to narrow the tab you are on, so a long list stays easy to get through.
- Back or the arrow closes search and puts your full list back.
- Your total entry counts live on the Profile screen, under your statistics.
- The system back button now works everywhere in Settings: Appearance, Navigation, Language, Browser, the legal pages and licences all return to Settings instead of leaving the app.

## 1.3.5
**A clearer top bar, and news beyond your list**

- The top bar sits tighter under the status bar, and the logo and bell are now as large as the selected tab below - easier to see and to tap.
- The bell shows a dot in your accent colour when something new is waiting, and it clears as you read.
- New setting: "All news". Turn it on under Notifications to hear about every MyAnimeList story, not only titles on your list.
- Episode discussions are now complete for tricky entries: sequels whose threads MyAnimeList files under a different spelling of the title, and older seasons whose discussions had gone quiet under a currently-airing sequel. The list now keeps looking until it has every episode.
- Fixed a startup crash on devices whose storage is full or damaged: the app now opens normally, and only background sync is skipped.

## 1.3.4
**All the discussions, in-app**

- "Show more" under Discussions now reveals threads in batches right in the app - no more being sent to the website to see the rest of a long-running show. The full MyAnimeList forum page is still one tap away under "More on MyAnimeList" as a fallback.
- Discussion matching is now truly universal: it works regardless of how the title is punctuated (brackets, quotes, "?", "☆", dashes...), so entries like [Oshi no Ko] and Kaguya-sama's OVA now show their threads.
- Faster, lighter on data: discussion search stops as soon as it has all the episodes, and the app now paces its AniList requests a touch higher while backing off automatically if the server ever asks it to - fewer stalls, no wasted quota.
- Opening an anime is much lighter on the network: the full cast and staff lists are now loaded only when you tap "More", so a normal detail view makes far fewer requests and pages open quicker.
- Fixed a crash on devices without a browser or share app: opening a link externally, sharing a title, or tapping a widget card now fails quietly instead of closing the app.
- Smoother and faster across the board, especially on mid-range phones: screens are now pre-compiled instead of being built the first time you open them, and cover art is cached properly - so less stutter, quicker detail pages, and much less repeated downloading.
- The back gesture now follows the modern Android animation.
- Icons that point somewhere - like "open in browser" - now face the right way in right-to-left languages such as Arabic, Persian, Hebrew and Urdu.
- Your sign-in is now protected by our own Android Keystore encryption instead of a library Google has retired. You stay signed in; nothing to do.
- The score on a detail page always stays on one line.

## 1.3.3
**English titles + a tighter, easier navigation**

- New setting: choose your title language. Turn on English titles in Settings › Appearance to see titles in English (where available) instead of romaji, everywhere in the app - instantly.
- The top bar is slimmer, so content starts higher and less space is wasted.
- The revolver navigation is shorter and now the whole tab area is tappable, not just the button - much easier to hit.

## 1.3.2
**Complete episode discussions**

- The Discussions list on a detail page now finds every episode/chapter thread, not just some: it pages through the full forum search, so long-running and multi-season series no longer drop scattered episodes.
- Discussions are now matched across the ways a title and its threads can differ - spacing or a dash ("Kyousou Giga" vs "Kyousougiga", "B-gata H-kei" vs "B Gata H Kei"), a quoted/movie title ("Bungaku Shoujo" Movie), a decorative symbol (Mahou☆Shoutengai), a "Movie 1 -" style label before a subtitle (Ars Nova Movie 1 - DC), or a different official translation - which previously hid the whole list, while threads that belong to a different entry (a "(TV)", "(OVA)", season or year tag) are still correctly kept out.
- The Discover search now resets to the browse view when you switch tabs and come back, instead of staying on your previous results (your recent-search history is kept).
- Screens no longer fail on a single hiccup from MyAnimeList's servers: a transient timeout (502/503/504) is retried automatically before an error is shown.

## 1.3.1
**Swipeable news + polish**

- Swipe left or right on the News screen to move between categories - the same fluid tab experience as My List and Seasonal, with the tag bar following your swipe.
- Voice actors now show their real language: a Chinese-original anime's lead now correctly reads "Chinese" instead of a stock "Japanese" label, everywhere on the detail page. Cast cards always pick the original-language actor (Japanese, then Chinese, then Korean) so a page never mixes languages, and the Dub field now lists the original audio too (e.g. "JA, EN, DE").
- Fixed notification images sometimes growing far past their intended size when the title wrapped onto several lines - every poster is now the same size.
- Home now loads noticeably faster on large lists: two heavy pieces of duplicate work at startup and on every return to Home were eliminated.

## 1.3.0
**Notifications that don't get lost**

- Episode alerts now recover on their own after a restart or an app update - you no longer need to open the app for them to keep working.
- On supported devices, alerts are pinned to the exact air time with a system alarm, so they arrive on schedule even with battery saving active.
- No more silently missed episodes: aired episodes are now also matched by their database ID over a catch-up window, so a title-name quirk or a delayed background check can't skip one anymore.
- If your device's battery settings are limiting alerts, Settings now shows a fix-it shortcut under Notifications (it disappears once everything is allowed).

## 1.2.9
**See every dub**

- Character pages now list the character's full voice cast at the bottom - every voice actor in every language, not just the Japanese one. Tap any of them to open their page.
- Anime detail pages now show which languages a title has been dubbed in, as short codes (EN, DE, ES...) right in the info grid - loaded together with the rest of the page, so nothing pops in or shifts while you read.

## 1.2.8
**On-time episode alerts + polish**

- New-episode notifications now arrive minutes after the episode actually airs: alerts are scheduled to each episode's real air time instead of waiting for the next background check, which battery saving could delay for hours.
- Reordering the navigation bar (in Settings or during the intro) no longer refreshes the screen when a row crosses the tab you're on - the list just moves.
- Home no longer flickers when you come back to it: it opens cleanly at the top, the same fix Seasonal and My List got.
- News categories now match MyAnimeList exactly: articles are filed under Anime, Manga, People, Music, Events and Industry using MAL's own article tags whenever the feed provides them.

## 1.2.7
**Grid columns + portrait lock**

- You can now choose 2 or 3 columns for the My List grid, from Settings under My List (it appears when Grid is selected), so the covers can be bigger and fit your phone better.
- The app now stays in portrait like the official MyAnimeList app, so rotating the phone no longer breaks the layout. Trailers and theme songs still go fullscreen (upright in portrait) and rotate to landscape when you turn the phone.

## 1.2.6
**Forum links and @mentions work like on MAL**

- Fixed forum posts showing raw [url=...] markup with a dead link when someone linked a YouTube video: those now render as proper tappable links, exactly like on MyAnimeList (only [yt] tags embed a player).
- @username mentions in posts are now tappable and open that user's MAL profile, just like on the web forum.
- Plain URLs pasted as text are now tappable links too (MAL web auto-links them; now so do we).
- Quoted link targets ([url="..."]) no longer break the link.
- [size=...] text sizing in posts now actually applies (it was silently ignored), including nested sizes; [sub]/[sup] now render as real subscript/superscript.
- News now always starts at the top when you open the tab or switch categories, instead of restoring a mid-list scroll position.

## 1.2.5
**Proper back inside the Seasonal Archive**

- Opening a season from the Archive now shows a back arrow to the left of the type filter, and pressing back (button or system) returns you to the Archive list instead of jumping to This Season.

## 1.2.4
**Smoother Seasonal grid**

- Changing the season, type filter, sort or its direction no longer flickers: the grid now jumps straight to the top cleanly, just like My List.
- Leaving Seasonal for another tab and coming back no longer flickers either: it is already on This Season, with no visible jump.
- The tab underline now glides when you tap a tab instead of jumping instantly.

## 1.2.3
**Seasonal back button + reliable return to this season**

- The back button now works on the Seasonal screen: from Last, Next or the Archive it steps back to This Season instead of leaving the app.
- Entering Seasonal now reliably lands on the current season every time, even after browsing the Archive.

## 1.2.2
**Seasonal: swipe between seasons + always opens on this season**

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