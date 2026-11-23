# CPE2600-LW11
**Program instructions**
$ make
$ ./mandelmovie -p (integer of child processes)
$ ffmpeg -i mandel%d.jpg mandel.mp4
$ xdg-open mandel.mp4
**End instructions**

**Program testing**
Note: all test were performed when my laptop was hovering at ~15% CPU usage and ~80% mem, these values never maxed out
process#	Time(s)
1	        532.897
2	        168.077
5	        93.833
10	      57.549
20	      50.639
Graphed data: https://github.com/user-attachments/assets/78e33d1c-2de3-496b-bbeb-f8bca89d348f
The graph gives the equation t=381.09x^-0.762 with and R-squared value of 0.9131
This equation isn't very accurate, observable in the lower R-squared value, but still gives a good representation to the change in time depending on the amount of child processes. This equation breaks very soon as once you try to use more than half the amount of values that need to be made, the program slows down. For example 50 processes takes more than a minute.

