You can set the volume on the micro:bit to make sounds louder or quieter.

You can find the `set volume`{:class='microbitmusic'} block in the `Music`{:class='microbitmusic'} menu.

<img src="images/music-menu.png" alt="The Music menu expanded, with the `set volume` block highlighted." width="350"/>

To use the `set volume`{:class='microbitmusic'} block, drag it above a `play`{:class='microbitmusic'} block.
In this example, a `play melody`{:class='microbitmusic'} block has been used inside an `on pressed`{:class='microbitinput'} block.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.setVolume(128)
    music._playDefaultBackground(music.builtInPlayableMelody(Melodies.Dadadadum), music.PlaybackMode.InBackground)
})
```

You can increase or decrease the volume by dragging the slider from left to right.

<img src="images/volume-slider.gif" alt="Animation showing the drop-down slider on the 'set volume' block. The value is clicked to reveal the slider and the volume is adjusted by moving the slider to the left or right." width="350"/>

### Setting the volume for V1 users

If you are using a micro:bit V1, there is no speaker to play the sounds, instead you have to attach headphones to the GPIO pins.

Take a look at the [guide from micro:bit to help you attach your headphones](https://makecode.microbit.org/projects/hack-your-headphones/make){:target="\_blank"}.
