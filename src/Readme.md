Welcome to the src/ directory. In here you'll find pretty much everything related to Audacity's functionality. 

* app/ contains the most basic backend, including CLI flags, shortcuts and basic color configs. 
* appshell/ contains everything related to the window you see that's not the project scene. Toolbars, dialogs, etc.
* au3audio/ contains the Audacity audio engine, based on PortAudio. This engine is somewhat legacy and is scheduled for replacement with the Musescore Studio engine at some point in the future, once that is sufficiently developed. 
* au3wrap/ contains the wrapper for Audacity 3 legacy code. All code depending on this wrapper (living inside various au3/ subfolders, usually) is due to be refactored at some point. 
* context/ contains the various contexts handlers - eg. pressing space does something different in a text input context vs in a playback context.
+ effects/ contains Audacity's various effects, as well as plugin implementations. 
* framework/ is the shared UI framework between Audacity and MuseScore Studio. Most of it gets imported and not locally defined here.
* playback/ contains all features and functions relating to playback. 
* project/ contains everything related to project loading and saving.
* projectscene/ contains the elements you actually interact with when editing a project - clips, cursors, timeline ruler, etc.
* record/ contains all features and functions related to recording.
* trackedit/ contains basic track editing interactions (eg. clipboard and undo history)