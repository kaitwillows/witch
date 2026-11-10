# music library organization but good

hi this project is WIP so the readme is all over the place atm. i just want to learn rust and such yeah.




this is a wip project that makes organizing a music library easier, though it may be biased towards my own needs.

## why this is needed

there are many reasons, but *some* baseline automation is almost necessary:

i like to collect *.flacs, not because they sound better than decent *.mp3s (they don't), but because it future proofs the ways in which i can transcode them in the future (also it feels cool to have the "exact" version of the song anyways)

immedietly, this standard makes it very impractical to not use at least some form of automation, as i don't believe LAME or ffmpeg have a native way to transcode in bulk, preserve directory structure, and preserve metadata. also lowkey every time i use ffmpeg, i have to use a cheat sheet its so esoteric idfk.

probably just going to start from that one basic task. hopefully i can expand the tool to a sort of system 


- project goals
  - [ ] convert a folder of flacs to LAME mp3 v2, keeping metadata and file structure exactly as-is
  - [ ] name/move files based on metadata tags
  - [ ] create database system for ensuring exact metadata
    - [ ] implementation details? plaintext or proprietary db? version controlled? git tracked????? custom version control system???!?!?!?! 
  - [ ] query external sources for metadata correctness
    - [ ] is the tracklist the same, and complete
    - [ ] is each song exactly the song it says it is 
  - [ ] allow for "webs", relating different songs by their writers, features, whatever

***

yapping and word vomiting lowkey:

witch is a local music organizational tool designed to quickly and easily ensure 

idfk its the nixos of music, but hopefully easier and faster to use


- for people who collect audio files, organizing them is often a tedious process, especially if you're picky like me and you want:
	- a specific directory structure
	- a specific file naming convention
	- specific metadata conventions
		- (maybe you want the "genre" tag to function as playlists)
        - maybe you want to ensure things like genres aren't there
        - maybe you want artists, collab artists, and featuring artists to be denoted a certain way
    - to know ALL of your metadata is actually correct
    - to know your flac files are actually flacs
    - to transcode your entire library into a specific format
    - to know that changes to your preferences can easily be accommodated for by an automated system that does exactly what you want it to
- witch uses both "source" files, 
