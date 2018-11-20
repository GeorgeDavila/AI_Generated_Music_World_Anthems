# AI_Generated_Music_World_Anthems
Using AI to generate novel music. Use national anthems as training data aiming for a sort of AI-generated 'World Anthem'. At least one the robots will like. Mainly based on music generating AI I worked on previously. 

## Training Data
Downloaded national anthems from sites listed below. Anthems are public domain, so good to use as training data. Use two main audio file types: MP3 and MIDI.


## MP3 format 
MP3s are higher-fidelity but bit harder to work with for our purposes. MP3s of course are just direct recordings, so they capture the subtleties of the music much better. However, this added complexity makes it harder to train AI on them. 

MP3 Anthems sourced from http://anthemworld.com required manual download so only picked a few, mainly larger population, nations. More training data the better, please feel free to let me know if you have all of them in mp3 format, will credit accordingly.  

Included EU and AU anthems in this set to give a bit more representation. 

## MIDI format
MIDIs play the notes of songs using an electric piano type sound. Plays just major notes, whereas in real music/sound there are obviously plenty of subtle frequency transitions. But their relative simplicity makes it a bit easier for our AI to work with them, expect a more intelligible output for this reason.

MIDI Anthems sourced from http://www.midiworld.com/search/5/?q=national%20anthems Which has 136 anthems listed, so about 60 nations are still missing from this set. Easier to download from here but still had to do it manually, so please let me know if I missed anything. Careful if you use it yourself, some of the last ones are unofficial renditions and anthems. 

### Visual Representation
MIDI files can be assigned a visual representation of a sequence of lines as shown in the image below. If we so chose we could take the midi files as pure images, use tensorflow image recognition techniques to analyze the images and generate new images (with a choice to fill in or erase boxes containing irregularities such as curves) which would be our new music. Don't do that here but its something to explore. Perhaps irregularities such as 'curves' generated mightbe regarded as the transition sound frequencies that we would hear in actual music. 

<table class="image">
<div align="center">
    <img src="http://www.musicarta.com/images/MP_page_illus_27.jpg.pagespeed.ce.036eLKYkJz.jpg"/>  
    <br>  
    <em align="center"></em>  
</div>
</table>

### Tensorial Representation
Could alternatively assign notes at each time step a binary value so that each time step is represented by a vector of note on/off modesThis would give us a tensor of 0's and 1's for each musical piece and a greater tensor of all these pieces to train our data on. Would then get tensor outputs based on patterns our ML model parsed out. 

I would imagine some audio software do treat MIDIs as tensors in this manner or a similar manner, but not too familiar obtaining such tensors from the files.


## Misc
There are philharmonic albums of their  renditions of the anthems and things like that. I don't use those here because 1) costs money 2) may not classify as public domain same way regular anthems do and 3) the AI may pick some of the style of the philharmonic, not capturing as much uniqueness of each anthem and making the AI a bit less robust. 
