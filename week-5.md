# Week 5

#### Task 1:  
<ins>Metadata Schema</ins>  

| Metadata | MEI Elements |
| ------------- | ------------- |
| Title | [`<title>`](https://music-encoding.org/guidelines/v5/elements/title.html) |
| Artist/ Arranger/ Encoder | [`<persName>`](https://music-encoding.org/guidelines/v5/elements/persName.html) |
| Publisher | [`<publisher>`](https://music-encoding.org/guidelines/v5/elements/publisher.html) [`<corpName>`](https://music-encoding.org/guidelines/v5/elements/corpName.html) |
| Date | [`<date>`](https://music-encoding.org/guidelines/v5/elements/date.html) |
| Key | [`<key>`](https://music-encoding.org/guidelines/v5/elements/key.html) |
| Instrument | [`<perfRes>`](https://music-encoding.org/guidelines/v5/elements/perfRes.html) |
| Genre | [`<genre>`](https://music-encoding.org/guidelines/v5/elements/genre.html) |

#### Task 2:  
[Verovio - Because I Love You (Yoo Jae-Ha) with Metadata](verovio2.html)

<ins>Reflection</ins>  
The philosophy behind my decisions is to use the elements that directly spell out the Metadata as much as possible. When presented with the option between adding a bibliography section within the code to include the genre element, I chose to add it because I believe that it is easier to understand from a human point of view and allows for the computer to systematically go through each section as it should have if it had all the information for each element filled into the Metadata. One downside is that this increases the length of the code and potentially could increase the runtime and potential for mistakes in the code. However, this also sets up anyone who wants to add on more encoding data without having to recode the entire Metadata as the sections are properly labelled and in place instead of using other alternatives that could get the job done but might not be as digitally accurate as it is right now. I believe as with the purpose of encoding to ensure continuity of the pieces, following proper MEI standards allows for future encoders to have an easier time encoding more Metadata on top of the current information for a more comprehensive understanding of the piece.

[← Back to home](./)

