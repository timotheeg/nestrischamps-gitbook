# OCR and Calibration

If you have not setup your OBS browser source, please do so first:

{% content-ref url="../setup-obs-browser-source.md" %}
[setup-obs-browser-source.md](../setup-obs-browser-source.md)
{% endcontent-ref %}

OCR is supported in browser for both device capture and screen capture.

2 default game ROMs are supported:

| Classic Tetris                          | [DAS Trainer](https://www.romhacking.net/hacks/3761/) |
| --------------------------------------- | ----------------------------------------------------- |
| ![](<../.gitbook/assets/image (3).png>) | ![](<../.gitbook/assets/image (4).png>)               |

The fields that need to be OCR-ed per ROM are fixed (see highlighted areas above).

{% hint style="info" %}
There is a built-in automatic calibrator but it does not work too well, so you should always adjust the areas selected for calibration to be as close as possible to the desired outcome.
{% endhint %}

In both cases, go to [https://nestrischamps.io/room/producer](https://nestrischamps.herokuapp.com/room/producer), start a game at level 0 **before** you press the `Calibrate and Capture` button. In DAS Trainer, pause as soon as the game starts, then click the button. In Classic Tetris, click as soon as the game starts. In both cases, keep your fingers crossed that the auto calibrator takes you close to the desired state, and then fine tune all the capture areas to be pixel perfect.

Once calibration and tuning has been done, the capture window and the browser tab **must** stay focused (do not move to other tabs).

### Digits

The capture area should "hug" the digits on top, right, bottom, left, (using 0 as a reference), like this:

* ![Capture area for 2 digits](https://nestrischamps.io/docs/digits\_2\_0.png)
* ![Capture area for 6 digits](https://nestrischamps.io/docs/digits\_6\_0.png)

Note that if you calibrate something that starts with a 1, the captured area should NOT hug the one on the left (notice the black strip on the left).

* ![Capture area for 18](https://nestrischamps.io/docs/digits\_18.png)

### Preview

To calibrate the preview properly, run the calibration in level 0 over multiple pieces, such that:

* Pieces S, Z, L, J, T, O are "hugged" TOP and BOTTOM in the capture area![Capture area for S preview](https://nestrischamps.io/docs/preview\_s.png) ![Capture area for Z preview](https://nestrischamps.herokuapp.com/docs/preview\_z.png) ![Capture area for L preview](https://nestrischamps.herokuapp.com/docs/preview\_l.png) ![Capture area for J preview](https://nestrischamps.herokuapp.com/docs/preview\_j.png) ![Capture area for T preview](https://nestrischamps.herokuapp.com/docs/preview\_t.png) ![Capture area for O preview](https://nestrischamps.herokuapp.com/docs/preview\_o.png)
* Piece I is "hugged" LEFT and RIGHT in the capture area![Capture area for I preview](https://nestrischamps.io/docs/preview\_i.png)

"hugged" means there is no black border.

### Current Piece (DAS Trainer only)

To calibrate the preview properly, run the calibration in level 0 over multiple pieces, such that:

* Pieces L, J are "hugged" TOP ONLY in the capture area (notice there's a black strip at the bottom)![Capture area for L current piece](https://nestrischamps.io/docs/cur\_piece\_l.png) ![Capture area for J current piece](https://nestrischamps.herokuapp.com/docs/cur\_piece\_j.png)
* Pieces S, Z, T, O are "hugged" BOTTOM ONLY in the capture area (notice there's a black strip on top)![Capture area for S current piece](https://nestrischamps.io/docs/cur\_piece\_s.png) ![Capture area for Z current piece](https://nestrischamps.herokuapp.com/docs/cur\_piece\_z.png) ![Capture area for T current piece](https://nestrischamps.herokuapp.com/docs/cur\_piece\_t.png) ![Capture area for O current piece](https://nestrischamps.herokuapp.com/docs/cur\_piece\_o.png)
* Piece I is "hugged" LEFT and RIGHT in the capture area![Capture area for I current piece](https://nestrischamps.io/docs/cur\_piece\_i.png)

### Color (Classic Tetris only)

Reading colors from the frame helps matching the block colors when scanning the field.

The are 3 colors to read: color1, color2, and color3. They should be read from the pieces stats on the left by selecting one block from the T piece, J piece, and Z piece.

The blocks should be chosen like this

![Piece statistics panel highlighting color blocks](https://nestrischamps.io/docs/statistics\_colors.png)

The selection should not include any black border, but color1 should include the block's border. They should look like this:

* ![Capture area for color 1](https://nestrischamps.io/docs/color\_1.png)
* ![Capture area for color 2](https://nestrischamps.io/docs/color\_2.png)
* ![Capture area for color 3](https://nestrischamps.io/docs/color\_3.png)

### Field

To calibrate the field capture, try to stack pieces on the left, right, and bottom, and even all the way up on the top-left and top-right.

Having done that, hug the capture on right, left, top, bottom. do not leave black borders at the bottom and right! Like this:

![Capture area for field](https://nestrischamps.io/docs/field.png)

### Congratulations

Congratulations! You have made it 🥳

Untick `Show Parts` if you have not, to save some rendering power.

And remember, **always keep the producer in the foreground and keep it focused** when streaming, otherwise the performance will be horrible.
