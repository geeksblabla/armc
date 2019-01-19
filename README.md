# armc

DevC Casablanca resources for playing with Spark AR studio

## Devc-Casablanca Challenge

Use the fez model and it's texture to build a face tracker effect for facebook and instagram.

Resources are available in challenge folder, make sure to convert the texture to a supported image format for Spark AR studio.

Surprise us and post your creative idea in the group [devc-casa](https://www.facebook.com/groups/DevC.Casablanca/)

## Encoding audio

To be able to use audio in Spark AR Studio you will need to encode you audio file

Convert audio from stereo to mono

```bash
ffmpeg -i intial/Sahara_Rains.mp3  -ac 1 prepared/Sahara_Rains_mono.mp3
```

Then encore to `aac` using `libfdk_aac`

```bash
ffmpeg -i intial/Sahara_Rains.mp3  -c:a libfdk_aac prepared/Sahara_Rains_mono.m4a
```

Or if `ffmpeg` is not compiled with `libfdk_aac` support use the buildin `aac` encoder

```bash
ffmpeg -i prepared/Sahara_Rains.mp3 -c:a aac -b:a 192k  prepared/Sahara_Rains_mono.m4a
```

## Resources

Spark AR studio [website](https://www.sparkar.com/ar-studio/)

3D Modeling software [blender](https://www.sparkar.com/ar-studio/)

Animating characters [mixamo](https://www.mixamo.com)

Audio library [youtube](https://www.youtube.com/audiolibrary/music)