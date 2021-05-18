# blur-background-webcam-without-green-chroma

Free solution to put background blur on your webcam without using chroma. Designed for OBS Studio and others apps.

Intelligent and real-time detection of the person on the webcam. No need to set the blur zone manually.

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

1. Access to X URL and check the blurred background result in real time, with your webcam. You don't need to install anything.
2. Open OBS Studio from a Terminal, with the following 2 commands (path sample for Windows users, please check your OBS instalation path):
        cd C:\'Program Files'\obs-studio\bin\64bit\
        .\obs64.exe --use-fake-ui-for-media-stream

        If you don't have OBS installed yet, you can download it for free here: <https://obsproject.com/>
3. In the OBS scene, add a "Browser" item and indicate the previous URL (X).
4. That's all! Your webcam will appear in your OBS scene with a blurred background in realtime.

Now you can share your OBS scene as a virtual webcam and use it in other video conferencing applications that didn't have the background blur functionality. You can also stream directly with OBS enjoying blurred background on your webcam.