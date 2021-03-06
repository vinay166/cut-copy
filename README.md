# cut-copy

I've always loved David Bowie. His death affected me fairly strongly and brought me back into thinking about his methods of working. 

One of his techniques for song writing was using the cut-copy technique, originally used by William S Burroughs. The idea is that you have a song or poem and cut up and separate the various phrases, then bring them back together in a random fashion to create new ideas. 
William Burroughs and David Bowie have both said that this can often produce strange results, such as potential predictions of the future events.
(Check this out for more info: http://www.openculture.com/2015/02/bowie-cut-up-technique.html)

I took the cut-copy technique and wrote two python scripts to automate this with text or audio. 

#cut-up_txt.py:
This will jumble any text document and output a new one.
Run like this:
python infile.txt. It will create an output file and print to the screen

#cut-up_wav_randomize.py
This will take all wav files in the running directory and compile them in a random order into one wav file. I used the convenient library pydub (http://pydub.com/). It's easy to switch this to write to mp3 or other formats.

#cut-up_wav.py
This will take all wav files in the running directory and compile them in the same order each time you do it. 

#cut_sample.py
This will take one input wav, cut it up and mash it back together.
If you want different time slices, change the futureslice variable. 1000 = 1 second

Run like this: python cut_sample.py sample.wav

Output will be the filename you used with _sliced.wav after it.

# To run these, you need to install the following:
pip install pydub

brew install libav --with-libvorbis --with-sdl --with-theora