# blur-background-webcam-without-green-chroma

Free solution to put background blur on your webcam without using chroma. Designed for OBS Studio and others apps.

Intelligent and real-time detection of the person on the webcam. No need to set the blur zone manually.


Before | After (blur)
--- | ---
![before 1](images-tutorial/people-01.jpg "before 1") | ![after 1](images-tutorial/people-01-blur.jpg "after 1")
![before 3](images-tutorial/people-03.jpg "before 3") | ![after 1](images-tutorial/people-03-blur.jpg "after 3")


## Compatible with:
- All versions of **OBS Studio**.
- Modern web browsers.
- Windows.
- Mac OS.
- Linux.

## Features:

**You don't need to install anything** to use it in OBS Studio and have a blurred background on your webcam.

**No limit on frames per second (FPS)**. The maximum FPS will depend on the hardware of your computer. This uses artificial intelligence (TensorFlow + BodyPix) to detect the pose of your body and blur only the background. This processing is done locally on your computer.

The blurred background result is **similar to other video conferencing apps** like Zoom, Teams, or Google Meets. Similar to other premium apps.

## Steps to use in OBS Studio (Windows, Linux, Mac OS):

1. Access to <https://javiercampos.es/projects/blur-background-webcam/> URL and check the blurred background result in real time, with your webcam. You don't need to install anything.
2. Open OBS Studio from a Terminal, with the following 2 commands (path sample for Windows users, please check your OBS instalation path):
        cd C:\'Program Files'\obs-studio\bin\64bit\
        .\obs64.exe --use-fake-ui-for-media-stream

        If you don't have OBS installed yet, you can download it for free here: <https://obsproject.com/>
3. In the OBS scene, add a "Browser" item and indicate the previous URL (<https://javiercampos.es/projects/blur-background-webcam/>).
4. That's all! Your webcam will appear in your OBS scene with a blurred background in realtime.

Now you can share your OBS scene as a virtual webcam and use it in other video conferencing applications that didn't have the background blur functionality. You can also stream directly with OBS enjoying blurred background on your webcam.

## URL Parameters

You can customize the behavior of the background blur effect by using URL parameters. These parameters allow you to adjust the blur intensity, enable or disable mirroring, and configure the edge blur amount. If no parameters are provided, default values will be used.

### Parameters

1. **`blur`**:
   - **Description**: Adjusts the intensity of the background blur.
   - **Range**: `0` (no blur) to `100` (maximum blur).
   - **Default**: `100`.
   - **Example**: 
     - `?blur=50` (medium blur).
     - `?blur=0` (no blur).

2. **`mirror`**:
   - **Description**: Enables or disables horizontal mirroring of the video.
   - **Values**: 
     - `1` (enable mirroring).
     - `0` (disable mirroring).
   - **Default**: `1` (mirroring enabled).
   - **Example**: 
     - `?mirror=0` (disable mirroring).
     - `?mirror=1` (enable mirroring).

3. **`edge`**:
   - **Description**: Sets the blur intensity for edges between the person and the background.
   - **Range**: `0` (no edge blur) to `5` (maximum edge blur).
   - **Default**: `3`.
   - **Example**: 
     - `?edge=1` (low edge blur).
     - `?edge=5` (maximum edge blur).

### Combining Parameters

You can combine parameters in the URL to customize multiple settings at once. Separate each parameter with an `&`.

**Example**:  
`https://javiercampos.es/projects/blur-background-webcam/?blur=75&mirror=0&edge=4`

- `blur=75`: Medium-high background blur.
- `mirror=0`: Disable mirroring.
- `edge=4`: High edge blur.

### Default Behavior

If no parameters are provided, the application will use the following defaults:

- `blur=100` (maximum blur).
- `mirror=1` (mirroring enabled).
- `edge=3` (default edge blur).

### Notes

- Parameters outside their valid range will be ignored, and their default values will be used instead.
- The application ensures input validation to avoid unexpected behavior.

Try adjusting these parameters to find the best configuration for your needs!
