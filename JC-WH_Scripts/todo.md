# TO DO

Audio speach glitch??

(Atrium Arrive?) - Note: also printed "native(music) rate=44100" again; no obvious reason
E/daoplayer-engine( 7169): Error doing track write: null
E/daoplayer-engine( 7169): java.util.ConcurrentModificationException
E/daoplayer-engine( 7169): 	at java.util.TreeMap$MapIterator.stepForward(TreeMap.java:883)
E/daoplayer-engine( 7169): 	at java.util.TreeMap$BoundedMap$BoundedIterator.stepForward(TreeMap.java:1485)
E/daoplayer-engine( 7169): 	at java.util.TreeMap$BoundedMap$BoundedEntrySet$1.next(TreeMap.java:1513)
E/daoplayer-engine( 7169): 	at java.util.TreeMap$BoundedMap$BoundedEntrySet$1.next(TreeMap.java:1511)
E/daoplayer-engine( 7169): 	at org.opensharingtoolkit.daoplayer.audio.FileCache.update(FileCache.java:403)
E/daoplayer-engine( 7169): 	at org.opensharingtoolkit.daoplayer.audio.FileCache.update(FileCache.java:371)
E/daoplayer-engine( 7169): 	at org.opensharingtoolkit.daoplayer.audio.AudioEngine$PlayThread.fillBuffer(AudioEngine.java:310)
E/daoplayer-engine( 7169): 	at org.opensharingtoolkit.daoplayer.audio.AudioEngine$PlayThread.run(AudioEngine.java:221)
D/

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


## done


