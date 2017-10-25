# How to calculate Bremer indices in TNT
---

*Disclaimer*: These instructions are *not* official. They have been written by [Laura Rocha Prado](http://laura.rochaprado.com), and developed through documentation reading, lecture attending, and trial and error. They have been tested only in Windows environments. As a rule of thumb, to avoid errors in TNT, make sure your matrix is in the same folder as the `TNT.exe`, and you have extracted all the scripts from the `tnt_scripts.zip` folder there too.

## Step-by-step

1. Open your matrix.
2. Open you `.ctf` tree file containing your Most Parsimonious Trees (without the consensus).
3. Execute the below command sequentially, substituing the parameters:
```
sub N hold 2N*1000; bb=tbr fillonly; unique*;
```
where N is the number of extra steps desired.
4. Save the trees found to `.ctf` file.
5. Save the log to `.out`.
6. Go to menu option Trees -> Bremmer Support -> Relative.
7. Continue executing the command in step *3*, adding the number of steps sequentially, until you reach a point in the consensus where you don't see a `?` in the nodes, or the tree memory is full.
8. When ready, after going through steps *4* to *7* again, save the tree with the indices, pressing `M` on your keyboard, and choosing the `.emf` filetype.

*An example of routine to be followed would be*:
```
sub 1 hold 2000; bb=tbr fillonly; unique*;
sub 2 hold 4000; bb=tbr fillonly; unique*;
sub 3 hold 6000; bb=tbr fillonly; unique*;
sub 4 hold 8000; bb=tbr fillonly; unique*;
sub 5 hold 10000; bb=tbr fillonly; unique*;
sub 6 hold 12000; bb=tbr fillonly; unique*;
sub 7 hold 14000; bb=tbr fillonly; unique*;
sub 8 hold 16000; bb=tbr fillonly; unique*;
sub 9 hold 18000; bb=tbr fillonly; unique*;
sub 10 hold 20000; bb=tbr fillonly; unique*;
sub 11 hold 22000; bb=tbr fillonly; unique*;
sub 12 hold 24000; bb=tbr fillonly; unique*;
sub 13 hold 26000; bb=tbr fillonly; unique*;
sub 14 hold 28000; bb=tbr fillonly; unique*;
sub 15 hold 30000; bb=tbr fillonly; unique*;

```





