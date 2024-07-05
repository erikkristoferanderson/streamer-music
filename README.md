# streamer-music
Music for streamers that reacts to Twitch chat.

## Notes taken from a stream on June 26, 2024

design ideas for music on stream
- should sound good without chat
- should react to chat in interesting ways

prototypes:
- things like 123...21 -> melody
- emoji associated to melody
- viewers can save melody to emoji

tools
- streamer.bot
- Python
- Ableton live

chord progressions?


thinking about chord progressions
very basic C major, A minor alternating progression would allow a C pentatonic scale to sound okay over both chords, so chat could use numbers 123... mapped to those notes.

tempo
- rate of chats per minute maps to tempo of song

How does it work  
streamer.bot watches Twitch chat and sends chat message to a websocket (local)  
Python picks up messages from websocket server  
Python parses messages and sends MIDI signals  
loopMIDI carries midi signals on device  
Ableton reads the signals and plays virtual instruments  

side idea: sweep filters over 8 bars.  
chat controls on/off, direction of sweep  



questions for later:  
- how easy is it to overload a midi bus?  



concept:

ambient music, programmed in Sonic Pi, but chat can inject notes into a queue of notes, and that echoes through the ambient music in sonic pi  


live coding performance with some amount of chat input?  

side note: heat plugin for Twitch with maybe Godot?  
side note: ableton vs sonic pi  

- poll integration
- saved songs and switching
- musician signup (drums, bass, lead, samples)
- set patterns in song (notes or envelopes)
- modes: chaos or structured collaboration
- compression settings. also other effects
- reputation system for contributors
- instrument switching
- song saving
- song reloading (replay or continue to mutate)
- keep revisions of songs
- voting for "greatest hits" over given timeframe

"interactive stream toys"

how about generative art


how about: pendulum that draws with a pen, and longer chat messages have a larger impact on accellerating the pendulum, possibly in new directions

web page in docker container as OBS source.



