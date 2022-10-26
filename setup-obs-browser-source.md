# Setup OBS Browser Source

{% hint style="info" %}
This section assumes basic knowledge about [Streamlabs OBS](https://streamlabs.com/) and/or vanilla [OBS](https://obsproject.com/)
{% endhint %}

First, retrieve the `URL` of your favorite renderer from [https://nestrischamps.io/renderers](https://nestrischamps.herokuapp.com/renderers) (Twitch account required for registration).

Once you have it, create a `Browser Source` in OBS, and put the link of your favorite renderer into `URL`.

A 720p (1280x720) canvas at 60 `FPS` is recommended, which is a good compromise of real estate vs. draw time and upload bandwidth requirements. However feel free to try out 1080p (1920x1080) too if you feel adventurous.

The `Browser Source` setup should end up looking like this:

![OBS browser source configuration panel](https://nestrischamps.io/docs/streamlabs\_browser\_source.png)

Next, if you are a streamer:

{% content-ref url="streaming/ocr-and-calibration.md" %}
[ocr-and-calibration.md](streaming/ocr-and-calibration.md)
{% endcontent-ref %}

If you are a restreamer:

{% content-ref url="restreaming/administering-a-room.md" %}
[administering-a-room.md](restreaming/administering-a-room.md)
{% endcontent-ref %}
