# AeLyricTool
A simple, one-keyframe tool to easily make lyric videos, add subtitles, or provide CC using a single text layer containing your entire transcription.
Maybe I'll compile this into an actual plugin at some point and use github like a normal person, but for now I'm backing everything up like this.

**Overview:**
This tool is meant to provide nice looking text animations with minimal user input and is ideal for those needing to animate a lot of text, those looking for tools to add efficiencies to their workflow, and those new to the program.

Keyframes work slightly differently than usual, where typically if someone wishes to have a "step-wise animation" (e.g. hold value at 3 for 30 frames, switch to 7 at frame 31) you would need to set the keyframe interpolation, or if you're lazy like me, add a duplicate keyframe of the previous value one frame before when you want the change to occur.
Now, keyframes always behave as with the hold interpolation, so that step-wise motion between lines of text can be achieved without knowledge of interpolation.
In short, one just needs to set keyframes where they desire a particular line of text to animate on screen.

