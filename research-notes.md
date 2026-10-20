# DWLLRS — one of those nights | Similar Artists & Repertoire — research notes

Prepared by Keyman · access date 2026-10-20 · companion to `index.html`, `repertoire.csv`, `evidence.json`.

## Method

1. **Seed identity.** Apple Music album/song pages, Spotify album/track/artist pages (signed-out) and embed JSON, YouTube metadata via yt-dlp, Chartmetric track page (logged-in session). Versions kept separate: original single (2026-04-10), a second Spotify single listing with the same date, the summer version (Apple 2026-07-03 / Spotify 2026-07-10), and the album version (2026-07-10, track 1 of *tell you when you're older*).
2. **Fingerprint.** librosa 1.0.0 on the supplied WAV: tempogram, Krumhansl–Schmuckler key correlation on harmonic chroma, RMS/centroid/low-frequency share/percussive ratio/onset density in 10-second bins, agglomerative segmentation; ffmpeg ebur128 for loudness. No listening. Section labels were inferred by aligning a community chord chart to the energy boundaries.
3. **Playlist CSV audit.** 743 rows, 731 distinct trimmed name/curator pairs, 12 repeated pairs, 743 blank Country fields — all reproduced. Adds by month: Apr 412 · May 163 · Jun 91 · Jul 47 · Aug 25 · Sep 5. Name keywords: jesus 57, worship 49, christian 39, indie 14, summer 14, chill 16.
4. **Playlist resolution.** Top 12 by followers resolved through Chartmetric's playlists tab (name + curator + Spotify URL); smaller lists through Spotify search by name with the owner confirmed from the embed subtitle. Contents pulled from Spotify's public embed (first 100 tracks only).
5. **Candidate pool.** Shazam 'Similar songs' for the seed (17 items, IDs double as Apple Music song IDs), Apple Music similar artists (11), Chartmetric similar artists (page 1 of 30), playlist co-occurrence and adjacency across nine verified lists, playlist-name clues, and reciprocal Shazam lists of candidates.
6. **Verification.** Every accepted recording has its artist and release date checked on Spotify embed data and/or the iTunes Search API; identities from Spotify About text and press. Shazam supplied BPM/label/writers until it blocked requests.
7. **Rubric.** Sonic, vocal, mood/lyrical, audience overlap each High/Medium/Low/Unassessed; evidence confidence High/Medium/Low kept separate. Sonic and vocal capped at Medium because nothing was heard.

## Counts

- Artists investigated: 45 (plus 34 surfaced but unassessed)
- Artists accepted: 15 (faith-indie 8, indie-folk 5, alt-pop 2)
- Recordings accepted: 26 (High 5, Low 6, Medium 15)
- Playlists resolved: 15; verified co-occurrence with the seed: 9; context clues: 1

## Unresolved issues

- No listening. Sonic and vocal judgments are capped at Medium/Unassessed for every candidate, and the seed fingerprint is signal statistics aligned to a community chord chart.
- Playlist contents come from Spotify's public embed, which exposes only the first 100 tracks. Any placement beyond #100 (e.g., *JESUS* at #534, granola girl at #266) is resolved but not verified for co-occurrence.
- The export has no playlist IDs; identities were resolved by name + curator through Chartmetric (top 12) or Spotify search (small lists). Six names remain unresolved.
- Shazam blocked requests after about 25 pages, so BPM/label data covers 10 of 27 accepted recordings.
- Chartmetric similar-artist and comparable-track tables were read for page 1 only (Chrome extension disconnected before pagination).
- The '28-Day Change' column is a playlist-level Chartmetric field whose exact definition was not verified in-app; it is not song stream growth.
- Playlist follower counts are export snapshots and were never summed as an audience figure.
- Metrics are dated per platform and never combined across versions; the second Spotify single listing (35dPLCeXcr0ZuRAhOdS0a1) was not merged with the seed.
- Key: chord chart (D–F♯m–A–E, no capo) implies A major / F♯ minor; chroma correlation prefers C♯ minor. Needs an ear.
- Luke Rob identity: no bio; Viberate lists UK rock/folk-rock, Shazam tags Country, release via DistroKid-style imprint. Treated as partly resolved.
- 'christian music 🙌🤍' (janella): Chartmetric lists 278 tracks; the public embed returned 3 twice. Not used for co-occurrence.
- Chartmetric's artist overview still says 'signed to Island Records' while all 2026 releases are ℗ DWLLRS Records and the website footer still credits Island/4th & Broadway; the current contractual status was not verified and is not asserted in the report.
- YouTube: Chartmetric's 493.99K (Oct 19) is a multi-video total; the official audio alone showed 353,490 views on Oct 20. The mid-October jump is uncorroborated per video.

## Rejected and borderline candidates

| Candidate | Source | Status | Reason |
|---|---|---|---|
| Noah Kahan | Shazam similar ('Orange Juice'); Apple similar artist; MOODY INDIE co-placement ('Orbiter' #11) | borderline — reference anchor | Three signals but a mainstream act the client already knows; 'Orange Juice' (119 BPM) is about a friend's sobriety, not the seed's register. Kept out of the count so the list stays a discovery resource. |
| Forrest Frank | Adjacent to the seed in two playlists ('LIFE IS GOOD' #69; 'YOUR WAY'S BETTER' #6); #1 on three sampled lists | borderline — audience anchor | Strongest audience overlap in the faith lane, but sunny R&B-pop/CHH production and a solo rap-sung delivery diverge from the seed's melancholy alt-pop. Audience cannot override musical fit; link kept for context: spotify:track:3TQk8yZld28u3CvGiT8gHq. |
| Buffalo Traffic Jam | Shazam similar ('Buyin' Dirt'); cited in Noah Kahan's and Jonthekid.'s lists | borderline | Secular country-folk ('Sad tunes for degens'), 5.4M monthly listeners; vocal fit unassessed; no co-placement. Worth an ear test. |
| Daniel Leggs | Shazam similar ('Cassette', 120 BPM Pop) | borderline | Upbeat NYC alt-pop in the Arden Jones / Brotherr / Neon Dreams cluster; tempo and mood brighter than the seed. |
| mor | Shazam similar ('Fill My Lungs'); cited in Jonthekid.'s list | borderline | Capitol Nashville signing ('Father's Ending'); grief-driven acoustic songs — mood fits, but country tagging and no co-placement. |
| Bebe Stockwell | Shazam similar ('Nothing Good is Easy', 2026-10-09, Columbia) | borderline | Too new for placement evidence; indie-pop singer-songwriter; no sonic description found. |
| Jonthekid. | Shazam similar ('On My Knees (organ version)', 136 BPM, Hip-Hop/Rap tag) | borderline | Faith lyric and reciprocal similarity, but tempo and genre tag sit far from the seed; 11K monthly listeners. |
| Christian Leave | Shazam similar ('Please Notice', 2016) | rejected | A decade-old acoustic-pop viral single from an artist who has since moved to indie rock; era mismatch. |
| Cameron Whitcomb | Shazam similar ('Problem') | rejected | 'Rough-edged country, punk-leaning pop' (Spotify bio) — energy and voice far from the seed. |
| Neon Dreams | Shazam similar ('Take What's Yours', 75 BPM) | rejected | Its own similar list is South African pop; no overlap with the seed's graph beyond one edge. |
| Ashley Singh | Shazam similar ('Still Mine (Acoustic)', 69 BPM) | rejected | Slow piano ballad; Ike Dweck appears in its list, which is the only link to this report. |
| Brotherr | Shazam similar ('She'll Be Right on Time') | rejected | Three-track catalogue, 38K listeners, no bio; cannot be assessed. |
| Krooked Kings | Chartmetric similar artist (84%); Apple similar artist | unassessed | Artist-level similarity only; no track-level or playlist evidence. |
| slenderbodies · Bay Ledges · Mr Twin Sister · Dreamgirl · Sjowgren · Claud · Forrest Nolan | Chartmetric similar artists (79–85%) | unassessed | Chill indie/alt-pop set; no track-level evidence. A secular-lane watchlist, not recommendations. |
| Aidan Bissett | Apple similar artist; SAD VIBES co-placement ('my funeral' #66) | borderline | Alt-pop with two signals; 'my funeral' theme not verified. |
| Hans Williams · Stephen Dawes · Ethan Regan · HARBOUR · Bazzi · Dominic Fike | Apple Music similar artists | unassessed | Artist-level only. |
| Grace Runkle | Co-placed ×4; 'breaks my heart' in Gable Price and Friends' Shazam list | borderline | Worship-pop singer-songwriter ('I write songs with my Dad (the heavenly one)'); closer to congregational than alt-pop. |
| Elijah Thomas · Brothrly · Remnant House · GRAHAM · Ryan Ellis · Claire Leslie · Van Buren · Trey Simon · Mountain People Worship · LOST & FOUND · Tenroc · Common Noble | Co-placed in 2–4 sampled playlists | rejected from shortlist | Co-placement without any musical description or algorithmic link to the seed; most are worship or CHH. Listed so the co-occurrence table is complete. |
| Levi Troast · Chris Renzema · Jervis Campbell · Reagan James Broome · Tate Butts · Ivan Castro · Zach Webb | Neighbours in the lyric-named fan playlists or 'christian music 🙌🤍' | unassessed | Fan-playlist adjacency only. |
| Jonah Kegan · Benson Boone · Alexander Stewart · Zach Hood · Thomas Day | Playlist name ':) smile!' list titled with these artists (repeated pair in export); Thomas Day also in Arden Jones's Shazam list | unassessed | Name clue toward secular male pop; not investigated further. |
| SYML · Hazlett · Benjamin Steer · Brenn! · Hugo Barriol · Mark Ambor · Myles Smith · gavn! | MOODY INDIE / granola girl co-placement | unassessed | Secular indie-folk/pop neighbours on one list each; Brenn! 'Days On End' also appears in Noah Kahan's and Daniel Leggs's Shazam lists. |
| AZIEDOESNTEXIST · comehelpglo · Pink Boy · Ralph Castelli | SAD VIBES / ALTERNATIVE neighbours | rejected | Bedroom-pop / sad-alt with no documented fit; the seed is an outlier on that list. |
| Other DWLLRS recordings | Album 'tell you when you're older' (2026-07-10): dwellers, looking back at us now, driving (pt. 2), meet me on the roof, fed up, problems, another sad song, pretty for someone, remedy, mud, tell you when you're older, new spirits; plus 'Blue Spirits' (2022), 'Driving' (2023), 'Dividends' (2022), 'Nights That We Needed' (2024) | reference only | 'new spirits' (2026-06-05) is in Shazam's similar list for the seed and sits at #2 behind it in lena 🌻's fan playlist. Excluded from the similar-artist count by design. |

## Playlist resolution table

| Playlist | Curator | Export followers | Export position | Spotify ID | Status |
|---|---|---|---|---|---|
| Christian Pop Hits 2026 | Near Kingdom Records | 35.2K | 97 / 181 | 5emm12a7Q5EtFAI1xbiFUg | verified |
| that christian girl workout 🎧 | that christian girl | 118K | 68 / 174 | 4uorObp7TteQIcEf5wFHY8 | verified |
| Christian songs that make you wanna run, jump, sing and dance → now titled 'Upbeat Christian songs' | Jesse Frohling | 5,050 | 9 / 91 | 2MpHW3K3hgftpRklVslHox | verified (renamed) |
| SAD VIBES / ALTERNATIVE | @saiyanreece | 13.9K | 31 / 105 | 2Y8s6GKcsWIuMx3X4cG2hM | verified |
| MOODY INDIE | Landlake music | 7,466 | 18 / 51 | 1E74ArfjMNWg7eupRHPukH | verified |
| granola girl | abby dubinskiy | 13.2K | 266 / 281 | 5WlF7kbSNS4qEVRtXSlj9N | verified (other DWLLRS tracks visible) |
| Road Trip With Jesus🍃 | ARISE | 428 | 1 / 85 | 0fGnJqTizzXuVAIL0qu1pv | verified |
| Jesus turn the lights back on | M♡ | 191 | 1 / - | 2HjgrTZH9GJ5EkmFjvzcrM | verified |
| Jesus turned the light back on | tirs | 12 | 1 / 5 | 0LT5DrFywUFYTHC71gx4sG | verified |
| JESUS TURNED THE LIGHTS BACK ON! | lena 🌻 | n/a (not in export) | — | 0TMLNCDetkYcF9P6LonxiQ | context (not a Chartmetric placement) |
| *JESUS* | Ciara Chanel Self | 7,198 | 534 / 553 | 5k2AP8RaVkWfBwgI8FwyqO | resolved, seed not visible |
| christian music 🙌🤍 | janella | 41.5K | 276 / 556 | 2hwMrwtwOQgo3nSndcR2cw | resolved, contents inconsistent |
| niche sad girl christian songs | salty seas | 305 | 1304 / 1435 | 2vjAlyDU6enRVeVLYbMpZA | resolved, seed not visible |
| Songs that feel like starting over | Cora <3 | 830 | 193 / 199 | 0e0g1q9Qxy8VY14bw5cpxO | resolved, seed not visible |
| Christian Indie Hits | Alternative / Rock / Indie Pop | Near Kingdom Records | 17.4K (Chartmetric) | not a placement | 5dYLtetMfsHJlp8sbFh1aR | pitch suggestion (Chartmetric) |
| Pluto 🪐 · SUMMER FEELS(updated weekly) · Christian songs that feel like a vacation in your head · Songs to stare at the ceiling · abstract pop / new music playlist · Melancholie | various | 7,126 · 9,669 · 1,269 · 46 · 837 · 361 | various | — | unresolved |

## Source register

- **Supplied files** — Chartmetric screenshots (3) dated 2026-10-20; playlist CSV export (743 rows); WAV of the official audio — used for: Metrics, playlist placements, audio signal
- **Apple Music** — music.apple.com album 6768459373, song 6768459375, summer version 6784778228, album 6784779097, artist 1528133962 (similar artists) — used for: Release dates, genre, ℗ line, similar artists
- **Spotify (signed-out web player + public embed JSON)** — Track, album, artist and playlist pages; embed endpoint for track lists (first 100 tracks only) — used for: Play count, release dates, bios, monthly listeners, playlist contents, artist IDs
- **iTunes Search API** — itunes.apple.com/search — used for: Apple track IDs, release dates, genre tags for 50+ candidate recordings
- **Shazam** — shazam.com/song/… pages (blocked after ~25 requests; coverage partial) — used for: BPM, label, writers, 'Similar songs' lists (Apple Music recommendation graph)
- **Chartmetric (Hunter's logged-in Chrome session)** — Track playlists tab, playlist pages (current tracks with label/ISRC/streams), track and artist comparables, artist overview — used for: Playlist identity by name + curator, Spotify playlist IDs, similar artists, pitch suggestions
- **yt-dlp** — YouTube QuJY1vRIOow metadata — used for: Upload date, view count, description, tags
- **Ultimate Guitar** — tabs.ultimate-guitar.com/tab/dwllrs/one-of-those-nights-chords-6249281 (community chart) — used for: Chord loop and section structure; not an official source
- **Press** — Sweety High (2026-07-20); K-LOVE (2026-07-27); 94.7 The Word/GodTube (Living Again, Jul 2026); Atwood Magazine (2026-03-27); Artistrack (Gable Price and Friends); Liberty University (Beach Chapel); Whiskey Riff/Americana UK (Buffalo Traffic Jam); uDiscover (mor); Qobuz/AllMusic bio (DWLLRS) — used for: Attributed sound descriptions and identities

## Scope notes

- No external playlist or account was created; no one was contacted; no candidate audio was downloaded.
- Supplied files and existing report folders were left untouched.
- Popularity scores are omitted from the client-facing page.
