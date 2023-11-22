# Changes

I've removed kayboard lists that weren't QWERTY because I don't know Julia and it was a bit messy having to scroll past everything as I was debugging.

I've added the missing Swedish keys in what I think is the correct layout.

One big downside is that the Swedish keyboard heavily relies on the ALT GR key to type many special chars like {}, @ and ~, but the program only seems to support shift usage. I'm sure this is relatively easy to add but agian, I don't know Julia.

Currently the temperature is set to 1000 cause I changed out of curiosity and I just haven't changed it back.

uuuuh probably a bunch more.

I don't really get how the traditionalLayoutMap works but I added things until the program started lol.

Mostly all done out of curiosity.

# keyboards

Supporting simulated annealing code for the [Why I Made The World's Worst Keyboard](https://youtu.be/188fipF-i5I) YouTube video.

Written in Julia... because it's fast, easy to read, and annoys my labmates.

To run, download both filtes to the same directory and execute the Julia code. It should start by benchmarking your training data (myBook.txt) against QWERTY followed by building it's own optimal layout. Change the number of iterations and cooling rates as desired within the SA() function. The terminal will give some indication of current progres (also stored by a new text file will give a iteration-by-iteration record of progress), and .png files of the current best solution will be saved to your same directory.

To train on your own custom dataset either point the "myBook.txt" somewhere else or just replace its contents.

Good luck!
