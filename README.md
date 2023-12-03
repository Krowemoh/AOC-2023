# Advent of Code 2023 

This year I'm going to try and do the [Advent of Code](https://adventofcode.com) challenges in Pick BASIC! I've only ever gotten to day 7 so hopefully I'll get further along this year.

I'm also letting myself cheat after an hour or so as I don't want to get frustrated and give up the entire thing.

[My AOC Blog Posts](https://nivethan.dev/tags/advent-of-code)

## Set Up

I like to make it easy to get the day's puzzle so I have a routine called GET.PUZZLE.INPUT that will retrieve a puzzle input from the site and put it in a file called AOC-PUZZLE-FILE. I do a little bit of clean up afterwards because the puzzle input ends up with an extra blank line at the end.

Create the file:

```
CREATE-FILE AOC-PUZZLE-FILE 53,2,6 101,4,18
```

You can then update the GET.PUZZLE.INPUT routine with your session id, year and day.

The session id will need to be take out of the cookie.

```
Open a page in the browser (firefox)
Go to advent of code and be logged in.
Go to the puzzle and click the puzzle input.
Right click -> Inspect (on the plain text page)
Click the network tab in the newly opened window
Refresh the page
You should see the network request for the puzzle input
Click the network request
In the right hand side, there should now be various tabs.
Click the cookies tab
Double click on the session value
Paste this into the GET.PUZZLE.INPUT routine
```

Luckily this process doesn't need to be followed everytime as the session id does stay the same for awhile.
