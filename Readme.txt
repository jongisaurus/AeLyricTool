AeLyricTool
A simple, one-keyframe tool to easily make lyric videos, add subtitles, or provide CC using a text layer containing your entire transcription.
Maybe I'll compile this into an actual plugin at some point and use github like a normal person, but for now I'm backing everything up like this.
(Written in Ae v.17.1.3 build 41)

Alt. Download Mirror: https://drive.google.com/file/d/1Lp9YY5OuQqJADWaOLgjDV9zuE2IlNQVs/view?usp=sharing


Overview:
This tool is meant to provide nice looking text animations with minimal user input and is ideal for those needing to animate a lot of text, those looking for tools to add efficiencies to their workflow, and those new to the program.

Keyframes work slightly different from usual, where typically if someone wishes to have a "step-wise animation" (e.g. hold value at 3 for 30 frames, switch to 7 at frame 31) you would need to set the keyframe interpolation to hold, or add a duplicate keyframe of the previous value one frame before when you want the change to occur.
Now, keyframes always behave as with the hold interpolation, so that step-wise motion between lines of text can be achieved without knowledge of interpolation.
(This also allows any animations from the linear keyframe interpolation that is being visually suppressed)
In short, one just needs to set keyframes where they desire a particular line of text to animate on screen and the animation parameters will handle the rest.


How to Use:
First, you'll want to check the **"Text Edit Mode"** box on the **"TEXT CONTROLLER"** layer so you may enter your text (formatted with line breaks) into the **"SOURCE TEXT"** layer.
(I may set up automatic line breaks in the future if that seems useful)

The important part here is that you can paste your entire body of text.

Next, you'll want to place a keyframe with the **"Line number"** slider on the **"TEXT CONTROLLER"** layer (you may assume any keyframe animation I'm talking about is on this layer unless stated otherwise), and remember that the line enumeration starts at 0 (thanks zero-based indexing).

After that, it's all about changing the **"TEXT CONTROLLER"** settings to get the appearance and timing you're looking for.

For further customization, you can open the **"SOURCE TEXT"** layer dropdown and mess with the in and out animator ranges.
To "disable" an animator, you may delete it, but I would recommend setting it back to its default value just to be safe (e.g. scale = [100,100])

To have the text appear and disappear instantaneously without having to configure/disable all the animators, simply set the **"In/Out Animation Length"** slider to 0 (a zero second animation).

If you would like, I've included some simple text paths on the **"SOURCE TEXT"** layer, and you can animate those as you normally would.
(You'll need to un-hide and animate the word-based layer if you're using that; no current capabilities to parent those two together but won't be an issue if I simplify the expressions to only needing a single layer)

Lastly, if you wish to place the text/controller into another composition, you may do so by copy/pasting from the default **"TEXT"** composition.
(Just be sure to copy all three layers, there is a hidden one that handles the word-based animation)


Thank You:
I appreciate you checking out my expression template and I hope it could be of some use!

Making this work entirely through expressions was a little janky, so please let me know of any bugs (in my spaghetti code) that I overlooked!

If you have any questions/concerns feel free to message me on Twitter @BolideOfficial, and thanks again!

Also, if you'd like to support me the best way to do so is with the following link: https://ko-fi.com/bolide <3