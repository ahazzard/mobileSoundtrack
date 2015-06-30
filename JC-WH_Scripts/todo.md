# TO DO

`outward5`

- scene `Start/return` 
  - check/replace `routes['WH1-WH3'].nearest` -> `WollatonHallArrived`
  - check/replace `routes['WH_EP-EP_LTA'].nearest` -> `fixedPlaylistIn`
- scene `Start/any` 
  - check `routes['WH1-WH3']`? call `Start/return`?

- track `SisterCities_Drums`
  - check unitTime "unitTime": 6.1 -> 5.3?
- track `StellaVox`
  - check unitTime 7.7 -> 4.25?
  - remove section `mainBody`
- track `TheBadGuys`
  - check unitTime 8.593 -> 7.6?
- track `WaitingForGA`
  - check unitTime 8.484 -> 6.1?

## notes

scenes

`outward5` / `_JC-WH_startOut.json`

- `Start` -> `Start/any`
  - tracks: `holdingPad` (fade out)
- `Start/any` -> `track1/MitaDelMundo`, `track2/SisterCities`, `track3/NotAlone`, `track4/Stella`, `track5/TheBadGuys`, `track6/WaitingForGA`, `WollatonHallArrivalMusic`, `Start`
  - tracks: none
- `Return` -> `Start/return`
  - tracks: `holdingPad` (fade out)
- `Start/return` -> `WollatonHallArrived`, `fixedPlaylistIn`, `Return`
  - tracks: none

`outward5` / `JC-WH_adaptive_sceneOut.json`

- `track1/MitaDelMundo` -> `Start/any`, `track2/SisterCities`
  - tracks: `MitaDelMundo`, `holdingPad` (fade out)
  - "waypoints": {"W1": "J_CS", "W2": "J_CP", "W3": "WR"}
  - "routes": {"R1": "J_CS-J_CP", "R2": "J_CP-WR", "Rnext": "WR-WR_MR"}

tracks:

- `MitaDelMundo`: pauseIfSilent: true, unitTime: 4 (ok).


## script errors

D/daoplayer-service(12483): Log LOG_ERROR: Section **** refers to unknown next section mainBody
in:
`_JC-WH_SisterCities_multiTrackSections.json`
`_JC-WH_Stella_multiTrackSections.json`
`_JC-WH_TheBadGuys_trackSections.json`

## done

`outward5`

- scene `Start/return` 
  - replace -> `Start` (no gps) with `Return`
  - add scene `Return` (no gps)
- scene `Return` added
- scene `track1/MitaDelMundo`
  - 20s timeout for lost GPS
- all remaining scenes - 20 second timeout for lost GPS
- `_JC-WH_fixedPlaylist_tracks.json`
  - missing commas, line 25, line 76

