# find-dtmf
(sorry for my english, I'm not dumb but French)

You always dreamt to find the phone number dialled by someone in a video? It's now possible! You have to record the audio of the *beeps* and this script will extract phone numbers from the dial tones.

## Installation
(If you are on Mac or Windows, go to hell.)

```
git clone https://github.com/ribt/find-dtmf/
cd find-dtmf
chmod +x find-dtmf.py
sudo cp find-dtmf.py /usr/local/bin/find-dtmf
```

## Usage

You have to give a wav file (you can try to convert it with `ffmpeg -i audio.mp3 audio.wav` for example).

```
Usage: find-dtmf [-h] [-v] [-l] [-r] [-d] [-t F] [-i T] file.wav

optional arguments:
  -h, --help     show this help message and exit
  -v, --verbose  show a complete timeline
  -l, --left     left channel only (if the sound is stereo)
  -r, --right    right channel only (if the sound is stereo)
  -d, --debug    show graphs to debug
  -t F           acceptable frequency error (in hertz, 20 by default)
  -i T           process by T seconds intervals (0.05 by default)
```
