<h1>Vtuber Channel Stats Tracker</h1>
<h2>Goal:</h2>
To build a website which polls Youtube API every n seconds in compliance with the Youtube's acceptable query rate (10000 units per day, non updates cost 1 unit each.)
- Details are in https://developers.google.com/youtube/v3/determine_quota_cost

<h2>Requirements:</h2>
- This should fully utilize the daily quota elastically according to the number of channels registered to the app<br/>
i.e. hourly polling of 200 channels equate about 24*200 = 4800 polls a day<br/>
then p = 10000 / n where n = number of channels currently registered<br/>
- Store the polled data with date<br/>
- Display the stats on a ranking page<br/>
<br/>
For reference: 

[rank 1] channel name - subscriber count - n<br/>
[rank 2] channel name - subscriber count - n<br/>
[rank 3] channel name - subscriber count - n<br/>
...

<br/>
<br/>
Go API reference page: https://developers.google.com/youtube/v3/quickstart/go

