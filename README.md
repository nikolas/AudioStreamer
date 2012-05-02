ABOUT THIS PROJECT
------------------
This is a fork of sprhawk's fork of AudioStreamer (originally written by Matt Gallagher). It's purpose is mostly to add minor improvements, but also remove things I don't find important (shoutcast support and level metering, for instance, have been removed).

CHANGES
-------

- Added
  - Delegation (see the AudioStreamerDelegate protocol)
  
- Removed
  - Shoutcast support
  - Level metering code

- Improvements
  - Originally, after seeking, the audio from the old position would still play then suddenly cut to the new position, which was a bit jarring. Now, the audio cuts out immediately and begins playing once data has been buffered at the new position.