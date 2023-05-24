# Elevenlabs-Phrase-Recycler

Recycle Phrases from Elevenlabs - Store the first requested mp3, then use local files for subsequent same requests

Saves API clicks and runs faster

Put the two py files into: C:\Data\Python\VoiceFiles (The voice files will be saved to same folder)

Enter your Elevenlabs API key into 'say_or_fetch.py' (Get free one here: https://beta.elevenlabs.io/speech-synthesis )

Test it using 'say_or_fetch_TEST.py' - Enter the phrase you want

First time of running it will fetch the phrase from Elevenlabs

Subsequent requests will speak the file saved locally

You can adjust the speed of the saved mp3 - speed variable in say_or_fetch.py (short phrases tend to be spoken too quickly)

You can optionally set the voice when calling say_or_fetch.py, and a default voice is also set as a variable eg..
#

Usage Example - paste these two lines into any other python script to have it say a phrase:

from say_or_fetch import say_or_fetch

say_or_fetch("Hello, hope you're having a good day", "Bella")
#

You can optionally leave out the 'voice' argument and it will use default voice set in say_or_fetch.py

e.g.  say_or_fetch("Have a nice day")

