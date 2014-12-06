ParseHumanDate.js
=================

A Javascript library to parse human readable dates and times

> See demo [here](http://benwasser.com/parsehumandate.html).

This is basically an amalgamation of three existing human date/time parsers (datejs, chrono, and sugar). I found I needed to build this library because each of the existing ones has pretty big limitations and these three tend to compliment each others' strengths when combined.

Instructions
-----------------

Include the script in your HTML:
```html
<script src="ParseHumanDate.js"></script>
```
Call it on given text:
```javascript
parseHumanDate('now');
>>> Sat Nov 22 2014 16:15:17 GMT-0500 (EST)

parseHumanDate('in an hour');
>>> Sat Nov 22 2014 17:15:17 GMT-0500 (EST)

parseHumanDate('next friday');
>>> Fri Nov 28 2014 12:00:00 GMT-0500 (EST)

parseHumanDate('tomorrow at 3');
>>> Sun Nov 23 2014 15:00:00 GMT-0500 (EST)

parseHumanDate('Dec 18 2am');
>>> Thu Dec 18 2014 02:00:00 GMT-0500 (EST)

parseHumanDate('jan 7');
>>> Wed Jan 07 2015 12:00:00 GMT-0500 (EST)
```

Known Issues
-----------------
Doesn't do well with some English written-out numbers in certain syntaxes ('in ten minutes', 'twelve hours from now')


