# Info about Custome Widget Created

Custom Widget created by me as part of this Quest/Bunty is "StopWatch" and gave the name of the widget also as Stopwatch. 
And kept the widget on the left side of the app using "left-widget" option and hence this widget easily got fit in the app with other widgets (i.e. "Date and Time" and "Calender")

# Custom Widget functionality

In Stopwatch Custom Widget, have the following parts:
- Watch "0:00:00:00" in "hours: minutes: seconds: millisec" 
- Start/Stop Button. If we press Start Button the same button will change to Stop Button & Watch will start ticking. When Stop Button is pressed, same button will switch to Start and the watch will stop ticking.
- Reset Button: By clicking the Reset button watch will reset to "0:00:00:00"

This widget is used style by using "stopwatch.css" style under "styles" folder. Keeping "Green" Color for Start/Stop Button and "Red" for Reset Button (for clear understanding to the user)
Also, like other widgets, it has "Close" & "+Add Widget" options. "Close" will close the widget and "+Widget" option will provide the option to add another widget on the web page.

# Logic of Custom Widget:  MyCustomWidget.js"

In the useEffect hook, we use setInterval to increment the time every 10 milliseconds. The clearInterval function is returned in the cleanup function to stop the interval when the component unmounts. 
The rest of the code logic has been explained using comments in "MyCustomWidget.js" File.

Also like other widgets, it is showing a prompt to the user, if the user tries to add Stopwatch Widget more than once. So, the new custom widget follows the basic standard of all other widgets