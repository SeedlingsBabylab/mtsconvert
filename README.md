# mtsconvert


This script crawls a directory tree and converts all MTS video files into mp4 video files. It will only convert
files that are in a directory that has "Eyetracking" somewhere within the path name (before the file itself). For example:

```
~/folder1/folder2/Eyetracking/folder3/folder4/video_file.mts
```
Will be converted. So will this:

```
~/folder1/folder2/Eyetracking/video_file.mts
```

These will not be converted:

```
~/folder1/folder2/video_file.mts
```

```
~/folder1/folder2/video_file.mts/Eyetracking/folder4
```

Notice that the "Eyetracking" must come before the video_file.mts

### usage

```
$: python mts2mp4.py start_dir
```
