# somebashscript

The purpose of this task is to find bots inside huge logfile.

Lots of bots logged in to our service. They all do same thing very quickly, they log in, change password and log off all within one second. We want to find them in log.

Please write command in bash that will show all profiles meeting following criteria:

- user logged in, user changed password, user logged of within same second (all 3 actions have to be done within 1 second)
- those actions (log in, change, log off) happend one after another with no other entires in between

fxsciaqulmlk - is typical profile name from the log file

small part of the log file

[a lot of data]
Mon, 22 Aug 2016 13:15:39 +0200|178.57.66.225|fxsciaqulmlk| - |user logged in| -
Mon, 22 Aug 2016 13:15:39 +0200|178.57.66.225|fxsciaqulmlk| - |user changed password| -
Mon, 22 Aug 2016 13:15:39 +0200|178.57.66.225|fxsciaqulmlk| - |user logged off| -
Mon, 22 Aug 2016 13:15:42 +0200|178.57.66.225|faaaaaa11111| - |user logged in| -
Mon, 22 Aug 2016 13:15:49 +0200|178.57.66.215|terdsfsdfsdf| - |user logged in| -
Mon, 22 Aug 2016 13:15:49 +0200|178.57.66.215|terdsfsdfsdf| - |user changed password| -
Mon, 22 Aug 2016 13:15:49 +0200|178.57.66.215|terdsfsdfsdf| - |user logged off| -
Mon, 22 Aug 2016 13:15:59 +0200|178.57.66.205|erdsfsdfsdf| - |user logged in| -
Mon, 22 Aug 2016 13:15:59 +0200|178.57.66.205|erdsfsdfsdf| - |user logged in| -
Mon, 22 Aug 2016 13:15:59 +0200|178.57.66.205|erdsfsdfsdf| - |user changed password| -
Mon, 22 Aug 2016 13:15:59 +0200|178.57.66.205|erdsfsdfsdf| - |user logged off| -
Mon, 22 Aug 2016 13:17:50 +0200|178.57.66.205|abcbbabab| - |user logged in| -
Mon, 22 Aug 2016 13:17:50 +0200|178.57.66.205|abcbbabab| - |user changed password| -
Mon, 22 Aug 2016 13:17:50 +0200|178.57.66.205|abcbbabab| - |user changed profile| -
Mon, 22 Aug 2016 13:17:50 +0200|178.57.66.205|abcbbabab| - |user logged off| -
Mon, 22 Aug 2016 13:19:19 +0200|178.56.66.225|fxsciaqulmla| - |user logged in| -
Mon, 22 Aug 2016 13:19:19 +0200|178.56.66.225|fxsciaqulmla| - |user changed password| -
Mon, 22 Aug 2016 13:19:19 +0200|178.56.66.225|fxsciaqulmla| - |user logged off| -
Mon, 22 Aug 2016 13:20:42 +0200|178.57.67.225|faaaa0a11111| - |user logged in| -
[a lot of data]
