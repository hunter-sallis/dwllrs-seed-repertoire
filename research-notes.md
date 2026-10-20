# DWLLRS — one of those nights | Similar Artists & Repertoire — research notes (rev 2, sound-first)

Prepared by Keyman · 2026-10-20. Rev 1 ranked by playlist and recommendation evidence; rev 2 re-ranks by measured acoustic distance after Hunter's feedback that rev 1 did not match the record's vibe.

## What changed

- With permission, 84 thirty-second Apple previews were downloaded and measured against the seed WAV (full track + verse/chorus/bridge windows). See `evidence.json → measurement` for every clip's score, components and raw features.
- Calibration: the seed's own preview scores 0.51; DWLLRS's catalogue lands at positions 5, 11, 12, 14, 26, 60, 63, 74 of 84.
- The fifteen accepted artists are now the fifteen closest measured, with a 'next five' and a 'what moved' table for the rev-1 scene picks.

## Method

Features were extracted with librosa from the supplied WAV (full track plus three 30-second windows: verse 0:19–0:49, chorus 1:15–1:45, bridge 2:11–2:41) and from Apple's 30-second previews of 80 clips: 71 candidate recordings plus nine DWLLRS recordings used for calibration. Each clip is compared to the seed on timbre (MFCC profile, weight 3), brightness (centroid, roll-off, high-band share, zero-crossing rate, 1.5), rhythmic density (percussive share and onset rate, 1.5), bass weight (1), dynamics (RMS spread and crest, 1), texture (flatness, contrast, mid-band, 0.75), major/minor lean (0.5) and tempo with octave and 3:2 tolerance (1). Lower score = closer. Calibration: the seed's own preview scores 0.51 against the full-track windows and ranks first of 80 clips; four of DWLLRS's eight other catalogue tracks (Nights That We Needed, the summer version, Blue Spirits, Dividends) land at positions 5, 11, 12 and 14, while the brighter 2026 album cuts (meet me on the roof, new spirits, pretty for someone) land at 26, 60 and 74. The metric tracks the DWLLRS sound of this record, not the band name. It cannot hear lyrics, vocal character or mood; those stay attributed.

## Measured ranking (all clips)

| # | Clip | Tag | Score | Closest on | Furthest on | BPM est | Brightness Hz | Bass share | Drum share |
|---|---|---|---|---|---|---|---|---|---|
| 1 | DWLLRS || one of those nights | seed | 0.51 | tone colour, brightness, bass weight, drum density, dynamics, major/minor lean, tempo | texture | 103 | 1813 | 0.04 | 0.28 |
| 2 | Jonthekid. || On My Knees (organ version) | cand | 0.93 | brightness, bass weight, drum density, major/minor lean, tempo | dynamics | 136 | 1466 | 0.08 | 0.34 |
| 3 | Dreamgirl || Teenage Blue | cand | 1.00 | bass weight, drum density, dynamics, tempo | tone colour | 92 | 1788 | 0.07 | 0.27 |
| 4 | Levi Collins || Ann Arbor | cand | 1.03 | bass weight, drum density, dynamics, major/minor lean, tempo | texture | 117 | 2018 | 0.08 | 0.27 |
| 5 | DWLLRS || Nights That We Needed | dwllrs | 1.07 | brightness, drum density, dynamics, tempo | major/minor lean | 108 | 1770 | 0.14 | 0.42 |
| 6 | Christian Leave || Please Notice | cand | 1.08 | bass weight, drum density, dynamics, tempo | tone colour | 112 | 1354 | 0.05 | 0.28 |
| 7 | Bebe Stockwell || Nothing Good is Easy | cand | 1.08 | brightness, drum density, dynamics, tempo | texture | 152 | 1532 | 0.20 | 0.30 |
| 8 | HAPPY LANDING || Wanderer | acc | 1.10 | brightness, drum density, dynamics, tempo | texture | 96 | 1305 | 0.19 | 0.37 |
| 9 | Sam Barber || The More I Hope | acc | 1.11 | brightness, dynamics | major/minor lean | 123 | 1499 | 0.16 | 0.31 |
| 10 | HAPPY LANDING || Radiate | acc | 1.13 | bass weight, dynamics, major/minor lean | texture | 89 | 1865 | 0.12 | 0.55 |
| 11 | DWLLRS || one of those nights (summer version) | dwllrs | 1.15 | brightness, dynamics, tempo | texture | 117 | 1526 | 0.18 | 0.45 |
| 12 | DWLLRS || Blue Spirits | dwllrs | 1.16 | brightness, bass weight, drum density, major/minor lean | dynamics | 129 | 1446 | 0.05 | 0.33 |
| 13 | Ike Dweck || Safe With Me | acc | 1.16 | drum density, dynamics, tempo | texture | 112 | 1997 | 0.15 | 0.38 |
| 14 | DWLLRS || Dividends | dwllrs | 1.16 | brightness, dynamics, tempo | texture | 112 | 1474 | 0.19 | 0.46 |
| 15 | Hans Williams || Skin | cand | 1.16 | bass weight, major/minor lean, tempo | texture | 103 | 1992 | 0.08 | 0.44 |
| 16 | Riverly || Fail and Fall | acc | 1.17 | bass weight, dynamics, major/minor lean, tempo | texture | 117 | 1902 | 0.13 | 0.39 |
| 17 | Bazzi || Myself | cand | 1.18 | bass weight, dynamics, major/minor lean, tempo | texture | 99 | 2178 | 0.10 | 0.55 |
| 18 | Hazlett || My Skin | cand | 1.18 | brightness, drum density, tempo | texture | 161 | 1590 | 0.17 | 0.28 |
| 19 | Joseph O'Brien || Looking Down | acc | 1.18 | drum density, tempo | texture | 92 | 1793 | 0.15 | 0.35 |
| 20 | Strings & Heart || peach sand | acc | 1.19 | bass weight, major/minor lean, tempo | texture | 161 | 2325 | 0.06 | 0.44 |
| 21 | Luke Rob || Distance to Close | acc | 1.19 | bass weight, dynamics, tempo | texture | 108 | 1970 | 0.12 | 0.42 |
| 22 | Hunter Metts || Weathervane | cand | 1.20 | brightness, tempo | texture | 144 | 1428 | 0.16 | 0.44 |
| 23 | Mr Twin Sister || Blush | cand | 1.21 | drum density, major/minor lean, tempo | texture | 144 | 1735 | 0.20 | 0.32 |
| 24 | Michael Marcagi || Scared To Start | cand | 1.21 | brightness, bass weight, tempo | major/minor lean | 152 | 1729 | 0.14 | 0.47 |
| 25 | SYML || The White Light of the Morning | cand | 1.22 | bass weight, drum density, major/minor lean | dynamics | 123 | 1072 | 0.06 | 0.18 |
| 26 | DWLLRS || meet me on the roof | dwllrs | 1.22 | bass weight, tempo | major/minor lean | 161 | 2323 | 0.07 | 0.45 |
| 27 | Mark Ambor || Belong Together | cand | 1.23 | bass weight, dynamics, tempo | texture | 92 | 2175 | 0.10 | 0.52 |
| 28 | Elijah Thomas || Nothing Like You | cand | 1.24 | drum density, dynamics, tempo | texture | 108 | 2228 | 0.15 | 0.35 |
| 29 | slenderbodies || king | cand | 1.24 | dynamics, tempo | texture | 99 | 1603 | 0.16 | 0.51 |
| 30 | Josiah Queen || demons | acc | 1.25 | bass weight, dynamics | texture | 129 | 2342 | 0.11 | 0.45 |
| 31 | Bennett Coast || Pretender | acc | 1.27 | bass weight, drum density, dynamics | major/minor lean | 89 | 2180 | 0.12 | 0.31 |
| 32 | Dominic Fike || 3 Nights | cand | 1.28 | dynamics, major/minor lean, tempo | texture | 152 | 2058 | 0.17 | 0.53 |
| 33 | Hugo Barriol || Glory Days | cand | 1.31 | major/minor lean, tempo | texture | 117 | 1803 | 0.17 | 0.36 |
| 34 | Ike Dweck || Dawn | acc | 1.31 | bass weight, dynamics, tempo | texture | 99 | 2644 | 0.10 | 0.44 |
| 35 | Luke Rob || Chapel Haze | acc | 1.32 | bass weight, dynamics, tempo | texture | 99 | 2141 | 0.11 | 0.53 |
| 36 | Krooked Kings || Catacombs | cand | 1.32 | major/minor lean, tempo | texture | 99 | 1803 | 0.18 | 0.53 |
| 37 | Bennett Coast || Now I Know You | cand | 1.33 | dynamics, tempo | texture | 172 | 2050 | 0.18 | 0.38 |
| 38 | Claud || Soft Spot | cand | 1.33 | tempo | major/minor lean | 161 | 2018 | 0.16 | 0.39 |
| 39 | Daniel Leggs || Cassette | cand | 1.34 | bass weight, dynamics | major/minor lean | 123 | 2081 | 0.03 | 0.34 |
| 40 | Hopeful. || Like I Am Yours | acc | 1.34 | dynamics, tempo | texture | 152 | 2375 | 0.12 | 0.47 |
| 41 | Reagan James Broome || Worth Dying For | cand | 1.35 | bass weight, drum density | major/minor lean | 123 | 2091 | 0.08 | 0.40 |
| 42 | Myles Smith || Stargazing | cand | 1.35 | drum density, dynamics | texture | 123 | 1995 | 0.17 | 0.44 |
| 43 | Brenn! || Days On End | cand | 1.36 | drum density, dynamics, tempo | bass weight | 108 | 1743 | 0.22 | 0.35 |
| 44 | Beach Chapel || Cardiff | acc | 1.37 | brightness | major/minor lean | 123 | 1672 | 0.15 | 0.65 |
| 45 | Josiah Queen || Garden in Manhattan | acc | 1.39 | dynamics, major/minor lean | texture | 123 | 2093 | 0.13 | 0.58 |
| 46 | Jet Trouble || Infinity | cand | 1.39 | bass weight, dynamics | major/minor lean | 129 | 2264 | 0.11 | 0.46 |
| 47 | slenderbodies || anemone | cand | 1.40 | dynamics, major/minor lean, tempo | texture | 117 | 1899 | 0.20 | 0.43 |
| 48 | Strings & Heart || flowers dressed in blue | acc | 1.41 | drum density, dynamics, tempo | texture | 161 | 2180 | 0.14 | 0.42 |
| 49 | Ralph Castelli || Right Hand to God | cand | 1.42 | drum density | texture | 129 | 1616 | 0.31 | 0.29 |
| 50 | Riverly || Safe and Sound | acc | 1.43 | dynamics, tempo | texture | 117 | 1974 | 0.15 | 0.58 |
| 51 | Beach Chapel || Woke Up | acc | 1.43 | bass weight, drum density, major/minor lean | dynamics | 89 | 2442 | 0.04 | 0.31 |
| 52 | Gable Price and Friends || One Bedroom Apartment | acc | 1.43 | drum density, tempo | bass weight | 144 | 1545 | 0.23 | 0.34 |
| 53 | Stephen Dawes || Sadie | cand | 1.44 | bass weight, tempo | major/minor lean | 112 | 2074 | 0.04 | 0.45 |
| 54 | Caleb King || Carpenter Boy | cand | 1.44 | bass weight, drum density, tempo | dynamics | 144 | 1899 | 0.06 | 0.24 |
| 55 | HARBOUR || Get You High | cand | 1.45 | bass weight, dynamics | major/minor lean | 86 | 2291 | 0.11 | 0.44 |
| 56 | Living Again || Cynical and Jaded | acc | 1.45 | dynamics | texture | 83 | 1893 | 0.16 | 0.46 |
| 57 | Tate Butts || My Defender | cand | 1.45 | dynamics | texture | 123 | 2126 | 0.17 | 0.38 |
| 58 | Thomas Day || she got a thing about her | cand | 1.46 | dynamics, tempo | texture | 117 | 2249 | 0.12 | 0.72 |
| 59 | Noah Kahan || Orange Juice | cand | 1.47 | drum density, tempo | tone colour | 117 | 1923 | 0.01 | 0.20 |
| 60 | DWLLRS || new spirits | dwllrs | 1.48 | dynamics, tempo | texture | 136 | 2028 | 0.18 | 0.48 |
| 61 | Living Again || Dive Into | acc | 1.49 | dynamics, tempo | texture | 144 | 2188 | 0.14 | 0.53 |
| 62 | Aidan Bissett || my funeral | cand | 1.51 | bass weight, tempo | texture | 92 | 2435 | 0.12 | 0.42 |
| 63 | DWLLRS || Driving | dwllrs | 1.52 | brightness, major/minor lean, tempo | dynamics | 96 | 1323 | 0.02 | 0.39 |
| 64 | Gable Price and Friends || Too Good | acc | 1.52 | tempo | major/minor lean | 172 | 2158 | 0.12 | 0.74 |
| 65 | Chance Peña || How Long, How Low? | acc | 1.52 | tempo | texture | 92 | 1212 | 0.23 | 0.57 |
| 66 | Ethan Regan || peach tree | cand | 1.53 | drum density | dynamics | 123 | 1776 | 0.01 | 0.23 |
| 67 | Chance Peña || i am not who i was | acc | 1.53 | drum density | bass weight | 129 | 1283 | 0.32 | 0.18 |
| 68 | Arden Jones || deadlove | acc | 1.55 | dynamics, major/minor lean | texture | 123 | 2628 | 0.13 | 0.37 |
| 69 | mor || Fill My Lungs | cand | 1.55 | dynamics, tempo | texture | 144 | 2657 | 0.14 | 0.39 |
| 70 | Sjowgren || Seventeen | cand | 1.57 | bass weight, dynamics, tempo | texture | 144 | 2420 | 0.11 | 0.46 |
| 71 | Buffalo Traffic Jam || Buyin' Dirt | cand | 1.57 | dynamics, tempo | texture | 144 | 2311 | 0.17 | 0.57 |
| 72 | gavn! || Good Terms | cand | 1.57 | tempo | texture | 152 | 2054 | 0.21 | 0.43 |
| 73 | Ryan Ellis || NO HALO | cand | 1.57 | tempo | texture | 161 | 2206 | 0.18 | 0.43 |
| 74 | DWLLRS || pretty for someone | dwllrs | 1.59 | bass weight, dynamics, tempo | texture | 152 | 2479 | 0.09 | 0.59 |
| 75 | Hopeful. || Everything Is Better | acc | 1.61 | bass weight, dynamics, major/minor lean, tempo | texture | 144 | 2786 | 0.09 | 0.69 |
| 76 | Bay Ledges || Safe | cand | 1.65 | tempo | texture | 103 | 2691 | 0.12 | 0.72 |
| 77 | Grace Runkle || open handed | cand | 1.68 | dynamics | texture | 129 | 1823 | 0.26 | 0.51 |
| 78 | Forrest Frank || LIFE IS GOOD | cand | 1.87 | major/minor lean, tempo | texture | 136 | 2459 | 0.19 | 0.80 |
| 79 | Sam Nicholson || Rule This Town | cand | 1.95 | dynamics, tempo | texture | 117 | 2826 | 0.14 | 0.75 |
| 80 | Forrest Frank || OKAY! | cand | 2.02 | major/minor lean, tempo | brightness | 117 | 3377 | 0.02 | 0.67 |

## What moved from rev 1

| Artist | Recording | Score | Rank/84 | Why it dropped |
|---|---|---|---|---|
| Gable Price and Friends | One Bedroom Apartment | 1.43 | 46 | Heavier low end (23% vs 4% in the verse), louder dynamics swing; a band record with a COIN sheen. Keeps reciprocal Shazam similarity and the best lyric fit in the pool. |
| Hopeful. | Everything Is Better | 1.61 | 66 | Bright surf-rock guitars (centroid 2.8 kHz vs 1.8) and the most drum-forward clip of the faith set (percussive share 0.69). Audience adjacency is real; the sound is not. |
| Living Again | Dive Into | 1.49 | 54 | Indie-rock drive, busier onsets, major-leaning. Adjacent to the seed in two playlists, far from it in sound. |
| Beach Chapel | Woke Up | 1.43 | 45 | 80s-synth pop-rock reads brighter and wider-dynamic than the seed; bass-light like the seed's verse but never settles. |
| Bennett Coast | Pretender | 1.27 | 25 | Major-leaning and brighter; Chartmetric's musicality call did not survive the preview comparison. |
| Chance Peña | i am not who i was | 1.53 | 59 | Lyrically the closest secular match, but the recording is bass-heavy (32% low share) and folk-rock brisk. |
| Arden Jones | deadlove | 1.55 | 60 | Brighter, busier alt-pop; the Apple/Shazam links point to audience, not texture. |
| Forrest Frank | OKAY! | 2.02 | 71 | Measures furthest of all: bright, drum-forward R&B-pop. Keep as the audience anchor of the Christian playlists, nothing more. |

## Limits

- Measurements use 30-second Apple previews for candidates and three windows plus the full track for the seed; previews usually cover a chorus, so verse textures are under-represented.
- The metric scores timbre, brightness, rhythm density, bass weight, dynamics, texture, mode and tempo. It does not hear lyrics, vocal character, melody or mood; those come from attributed descriptions.
- Six candidates had no Apple preview (Krooked Kings 'Headhunters', Forrest Nolan, AZIEDOESNTEXIST, Pink Boy, comehelpglo, Jonah Kegan) and are unmeasured. SYML was measured on a live version; Hopeful. and Arden Jones were re-pulled by ID after the search matched the wrong version.
- Playlist contents come from Spotify's public embed (first 100 tracks); placements deeper than that are resolved but not verified.
- Shazam blocked requests after about 25 pages, so BPM/label data from Shazam covers only part of the pool; tempos in the measured table are librosa estimates from previews and can land on 3:2 or 2:1 relatives.
- Metrics are dated per platform and never combined across the original, summer and album versions.

## Rev-1 notes (still valid for playlist resolution, CSV audit, identities)

See the rev-1 section of `evidence.json` (`rev1_evidence_based_ranking`, `playlists`, `csv_audit`) and the source register.
