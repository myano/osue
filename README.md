osue
====

Ohio State University's Emergency Page

Goal
----

This project contains commits of the index.html file located at 
http://ap.osu.edu/emergency/ over the course of the past few months.

This was created by running this in a cronjob:

    */10 * * * * DT=`date \+\%Y-\%m-\%d_\%H\%M\%S`; curl http://ap.osu.edu/emergency/ -o /home/yano/dev/osue/index-`echo $DT`.html

The interval which it runs has changed over time. Originally the project
started out pulling every minute to every couple of minutes to now settling
on once every 10 minutes.
