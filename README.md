Google-Translate-TTS
====================

A python script for using Google's undocumented TTS api to save text to an MP3 file.

For more background, check out this [blog post](http://www.hung-truong.com/blog/2013/04/26/hacking-googles-text-to-speech-api/).

```
usage: GoogleTTS.py [-h] [-o [OUTPUT]] [-l [LANGUAGE]]
                    (-f FILE | -s STRING [STRING ...])

Google TTS Downloader.

optional arguments:
  -h, --help            show this help message and exit
  -o [OUTPUT], --output [OUTPUT]
                        Filename to output audio to
  -l [LANGUAGE], --language [LANGUAGE]
                        Language to output text to.
  -f FILE, --file FILE  File to read text from.
  -s STRING [STRING ...], --string STRING [STRING ...]
                        A string of text to convert to speech.
```


Examples
===================

To convert text from a file:

```
GoogleTTS.py -f text.txt
```

To convert text from the commandline to a named file:

```
GoogleTTS.py -l ja -o konnichiwa_bitches.mp3 -s こんにちは
```

Extras
===

Dump File from Website
---
lynx -dump http://matrixfox.github.io/blog/2013/12/11/kali-linux-se-toolkit-social-engineering-toolkit/ > file.txt


Rip
---
python GoogleTTS.py -o out.mp3 -f file.txt


Remember
===================
Don't be evil.
