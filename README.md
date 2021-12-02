# reminder of how to add samples in Estuary

* create subfolder on github pages site
* copy aiff files in then convert to .wav
	* cd to directory, then

	* `for f in *.aiff; do ffmpeg -i "${f}" -vn -c:a pcm_s16le  -ar 44100  "${f%.*}.wav" ; done` 

* push changes in github desktop
* check files are there [https://github.com/tedthetrumpet/testpage/tree/master/samples]()
* use instructions [https://github.com/dktr0/estuary/wiki]() to create resources.json, or as below:
* go back up into the samples directory
* `cd ..`
* run the script like this: `/Users/jsimon/Dropbox/github_repositories/estuarystuff/generateAudioResources.sh . > resources.json`
* check the new local `resources.json` file then push using github desktop
* in Estuary terminal `!showresources`
	returns `0: reslist "samples/resources.json"`
* do `!reslist "https://tedthetrumpet.github.io/testpage/samples/resources.json"`
* to revert to default samples `!defaultresources`


# Maintaining and enhancing excellence in H1

> ‘a quotation’
    <cite>(reference 2021)</cite>

test check one two three some text here

[Link to page 2](https://tedthetrumpet.github.io/testpage/page2)

**Complexity:** recognising and dealing with the provisiional nature of knowledge, the application of knowledge in practice, conceptual complexity, and the complexity of learning process.


## References is H2

‘Polifonia’ Working Group on Artistic Research in Higher Music Education (2015) “Perspectives on 2nd Cycle Programmes In Higher Music Education” Association Européenne des Conservatoires, Académies de Musique et Musikhochschulen (AEC) <https://www.aec-music.eu/publications/perspectives-on-2nd-cycle-programmes-in-higher-music-education>

