# Week 3

#### Task 1:  
[Verovio - Because I Love You (Yoo Jae-Ha)](verovio.html)

#### Task 2:  
Here, I used 3 elements that appeared in both MEI and MusicXML files for the song (Because I Love You).

1. <note>
Firstly, <note> in MusicXML is much longer than in MEI. Its attributes (default-x, default-y) only describes where MuseScore drew the note on the page. However, the actual music like the pitch, length, and staff, is spelled out in a long list of child elements that must follow a fixed order. MEI does the opposite where the musical information like the pitch, length, and staff are packed into attributes on a single line. 
Next, their parents are different too. A MusicXML <note> can only sit directly inside a <measure>, and to show a chord it uses a little <chord/> tag which basically means "play this with the note before". In MEI, the notes sit inside a <chord> element, so the chord becomes one object and its length is written once instead of on every note.

I think MEI is much easier to read, although if I were to transcribe the song across 2 platforms like in Musescore, it definitely helps for it to look the same instead of just sounding the same. Afterall, musicians could make up one of the users and therefore it would be hard to read the score to play it. 

2. <staff>
Apparently, this element has different meanings in MEI and MusicXML. In MusicXML, <staff> has no attributes and no children so its just a number inside a <note> or <direction>, labelling which staff the note belongs to. In MEI, <staff> is a container that sits inside <measure>, carries an attribute n="2", and holds <layer> elements, which then hold the notes. So the implication is that MusicXML has to tag every single left-hand note with "staff 2" and even use a <backup> element to rewind time to the start of the bar before writing the left hand. MEI just puts the left hand in its own box. 

I think that MEI would then be more dependable in the recreation of the music information than MusicXML because the structure of MusicXML exposes it to many vulnerabilities. Should there be any mistakes in the code, the musiic will then throw the entire bar out of line. For a good safeguard, perhaps MEI and MusicXML could be used together to enable accurate visual transcribing while maintaining the integrity of the music.

3. <pedal>
In MusicXML, the <pedal> element is buried three layers deep (<measure> → <direction> → <direction-type> → <pedal>), and its attributes mostly describe whether it starts or stops and how it looks. In MEI, <pedal> sits directly inside <measure>, next to the staves, and its attributes state exactly which staff and which beat it applies to (staff="2", tstamp="1"). Neither has any children. What I found interesting is that MusicXML never states the timing, it is implied by where the pedal appears in the list of notes. So when Verovio converted my file, it had to work it out, and it chose tstamp="4.9" for every pedal release, which is basically a guess at "just before the barline". This shows that converting between formats is not simply copying. Some interpretation happens along the way. 

This begs the question: how many of these small decisions add up over a whole piece? Would someone reading only the MEI file know that 4.9 was a guess and not what I meant? Although accuracy of music is a subjective topic, it also brings up the issue of accurate representation as the music is converted to other versions using different tools and formats.

[← Back to home](./)
