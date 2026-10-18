# Week 3

#### Task 1:  
[Verovio - Because I Love You (Yoo Jae-Ha)](verovio.html)

#### Task 2:  
MusicXML VS MEI  
1. Key, time signature, and clef: MusicXML labels the items in seperate individual boxes while MEI compresses it into short tags on one line. MusicXML then positions the boxes into the bars, similar to how humans would read a score. Comparatively, MEI places it at the very beginning, dictating the key of the piece for everything else that follows after. Therefore, MusicXML requires the program to read the music to find the keys and clefs whereas it is instantly identifiable in an MEI file.
2. Notes and chords: Similarly, MusicXML has individual labels detailing the pitch, length, voice, and staff for every single note. MEI shortens the code with tags, where a series of notes played at the same time are nested in a <chord> folder. So MEI avoids repetition when reading through the code while MusicXML has a more lengthy process as it reads from the beginning of the bar again.  
3. Pedal and tempo: Pedal in MusicXML is wrapped in several layers of boxes with specific instructions on when the pedal is played while MEI uses one element <pedal> and tags to indicate when the pedal is being played. The timing of the pedal thus appears IN the list of notes while MEI states the exact beat <tstamp='1'> BESIDE the music. MEI becomes a more efficient manner of reading the music rather than just displaying the music.  
> MusicXML focuses on the visual aspect of a digital sheet music and mimics how a human would read the music while MEI prioritises efficiency and accuracy in the reproduction of the piece of music.

[← Back to home](./)
