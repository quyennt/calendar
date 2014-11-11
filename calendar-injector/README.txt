How to inject(example):
1.Inject public calendars:
	host:port/rest/bench/inject/CalendarDataInjector?userPrefix=abcuser000&fromUser=0&toUser9&createPublicCalendar=true&publicCalendarName=calendarName
2.Inject private events,tasks: 
	host:port/rest/bench/inject/CalendarDataInjector?date=MM/dd/yyyy&userPrefix=abcuser000&fromUser=0&toUser=9
 OR
	host:port/rest/bench/inject/CalendarDataInjector?injectMode=private&date=MM/dd/yyyy&userPrefix=abcuser000&fromUser=0&toUser=9
3.Inject public events, tasks in public calendars:
	host:port/rest/bench/inject/CalendarDataInjector?injectMode=public&date=MM/dd/yyyy&userPrefix=abcuser000&fromUser=0&toUser=0&publicCalendarName=calendarName
4.Inject public events, tasks in public calendars 
AND 
private events, tasks into default private calendar:
	host:port/rest/bench/inject/CalendarDataInjector?injectMode=both&date=MM/dd/yyyy&userPrefix=abcuser000&fromUser=0&toUser=9&publicCalendarName=calendarName

In 3 and 4: if the publicCalendarName does not exist, it will be created.	