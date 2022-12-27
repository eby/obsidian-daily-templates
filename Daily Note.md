---
day: <% tp.file.creation_date("YYYY-MM-DD") %>
weekday: <% tp.file.creation_date("dddd") %>
week: <% tp.file.creation_date("GGGG-[W]WW") %>
month: <% tp.file.creation_date("YYYY-MMM") %>
year: <% tp.file.creation_date("YYYY") %>
quarter: <% tp.file.creation_date("[Q]Q-YY") %>
tags: daily

status:
sleep:
energy:
stress:
focus:
productivity:
---
← [[<% tp.date.yesterday("YYYY-MM-DD MMM") %>|Yesterday]] | [[<% tp.date.tomorrow("YYYY-MM-DD MMM") %>|Tomorrow]] →

<svg viewBox="0 0 3650 100"> 
	<title>Timeline 2022</title> 
	<g class='bars'> 
		<rect fill='#E5E9F0' x='0' width='310' height='25'></rect> 
		<rect fill='#DDE1D8' x='310' width='280' height='25'></rect> 
		<rect fill='#BCCBBC' x='590' width='310' height='25'></rect> 
		<rect fill='#ACBFA4' x='900' width='300' height='25'></rect> 
		<rect fill='#CD7B74' x='1200' width='310' height='25'></rect>
		<rect fill='#D6726D' x='1510' width='300' height='25'></rect> 
		<rect fill='#C36863' x='1810' width='310' height='25'></rect>
		<rect fill='#D6726D' x='2110' width='310' height='25'></rect> 
		<rect fill='#B88B7F' x='2420' width='300' height='25'></rect>
		<rect fill='#BCCBBC' x='2720' width='310' height='25'></rect>
		<rect fill='#DDE1D8' x='3030' width='300' height='25'></rect>
		<rect fill='#E5E9F0' x='3330' width='310' height='25'></rect>
</g> 
<g class='labels' style="font-size:50px;" text-anchor="middle">
	<text fill='#3A3838' x='0' y='80' text-anchor="start">January</text> 
	<text fill='#3A3838' x='310' y='80' text-anchor="start">February</text>
	<text fill='#3A3838' x='590' y='80' text-anchor="start">March</text> 
	<text fill='#3A3838' x='900' y='80' text-anchor="start">April</text> 
	<text fill='#3A3838' x='1200' y='80' text-anchor="start">May</text> 
	<text fill='#3A3838' x='1510' y='80' text-anchor="start">June</text> 
	<text fill='#3A3838' x='1810' y='80' text-anchor="start">July</text> 
	<text fill='#3A3838' x='2110' y='80' text-anchor="start">August</text> 
	<text fill='#3A3838' x='2420' y='80' text-anchor="start">September</text> 
	<text fill='#3A3838' x='2720' y='80' text-anchor="start">October</text> 
	<text fill='#3A3838' x='3030' y='80' text-anchor="start">November</text> 
	<text fill='#3A3838' x='3330' y='80' text-anchor="start">December</text> 
</g> 
<g> 
	<circle cx= "<% tp.file.creation_date("DDD") %>0" cy="14" r="15" stroke="white" stroke-width="5" fill="white" /> 
	</g> 
</svg>

<br>

# <% tp.date.now("dddd, MMMM Do") %>.
**Gratitude List**:: 

## Rose, Thorn, Bud
**Rose**::
**Thorn**::
**Bud**::

> [!BRAIN]- Brain Dump
> Fill in here

> [!FOLDER]- Files Created Today
> ```dataview
> TABLE
>	file.ctime as "Created",
>	file.mtime as "Last Updated"
> WHERE file.ctime >= date(today)
> ```

> [!BUD]- Remember
 <% tp.web.daily_quote() %>