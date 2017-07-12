# Sort That Mess

**WARNING: This is a work in progress!** 

If you are like me you do not empty your camera's SD card after each photo session.
The SDs can store so many photos, why bother?

But when comes the time to save the photos somewhere, you have *one* directory with hundreds (thousands!) of photos. You have to sort that mess manually while crying and swearing that never again you will wait before transfering your photos.

This time is over! This small project is here to help!

The goal here is to write a small NodeJS script able to analyse the timestamps of your photos and automatically create subfolders.


## Algorithm: The logic behind

The timestamps of all the files is our one dimension data set.

In Machine Learning (BUZZWORD!) there are algorithms to solve this question: Clustering algorithms (BUZZWORD!). Their goal is to create group of data. But here we are working with one dimension only. Let's try something simple first:

+ The first very naive strategy I want to try is to compute the average time between 2 photos and group together the photos where the time between two photos is less than, say, 10 times the average.



## The main script

in your photos directory just call the script:

```
./sort-that-mess
```

The script will scan all the files and create a data structure of the timestamps.


## Future Improvements: 

### A web interface to visualize the groups

May be it would be nice to be able to see the timeline as a small chart and be able to split one group in several or, on the contrary, to merge several sub-folders in one.

