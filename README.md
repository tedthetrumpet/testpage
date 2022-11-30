# reminder to self of how to add samples in Estuary

* create local subfolder for github pages site
* make sure there are no spaces in the file names
* copy aiff files in then convert to .wav
	* cd to directory, then

	* `for f in *.aiff; do ffmpeg -i "${f}" -vn -c:a pcm_s16le  -ar 44100  "${f%.*}.wav" ; done` 

* push changes in github desktop
* check files are there [https://github.com/tedthetrumpet/testpage/tree/master/samples](https://github.com/tedthetrumpet/testpage/tree/master/samples) (or [https://github.com/tedthetrumpet/testpage/tree/master/nmsamples](https://github.com/tedthetrumpet/testpage/tree/master/nmsamples) for the main stable Naga Mas bank)
* use instructions [https://github.com/dktr0/estuary/wiki](https://github.com/tidalcycles/Dirt-Samples) to create `resources.json`, or as below:
* go back up into the samples directory
* `cd ..`
* run the script like this: `/Users/jsimon/Dropbox/github_repositories/estuarystuff/generateAudioResources.sh . > resources.json`
* check the new local `resources.json` file then push using github desktop
* in Estuary terminal `!showresources`
	returns `0: reslist "samples/resources.json"`
* do `!reslist "https://tedthetrumpet.github.io/testpage/samples/resources.json"` (or `!reslist "https://tedthetrumpet.github.io/testpage/nmsamples/resources.json"` for the main stable Naga Mas bank)
* to revert to default samples `!defaultresources`
