A. What's in injector:
	There are 2 parts in this injector:
	1. Default injection:
		- All parameters are defined in "configuration.xml" file.
		- Calendars, Events, Tasks are injected randomly. 
	2. Injection customize by TQA: 
		- All parameters are get from URL.	
		- Events & Tasks are injected into specific calendars with specific date.
B. How to inject:
		1. To use default injection:
				host:port/rest/bench/inject/CalendarDataInjector
		2. To use injection customized by TQA:
				2.1.Inject public calendars:
				host:port/rest/bench/inject/CalendarDataInjector?tqaCustomize=true&injectedUser=userId&createPublicCalendar=true&publicCalendarName=calendarName
				2.2.Inject private events,tasks: 
				host:port/rest/bench/inject/CalendarDataInjector?tqaCustomize=true&date=MM/dd/yyyy&injectedUser=userId
				OR
				host:port/rest/bench/inject/CalendarDataInjector?tqaCustomize=true&injectMode=private&date=MM/dd/yyyy&injectedUser=userId
				2.3.Inject public events, tasks in public calendars:
				host:port/rest/bench/inject/CalendarDataInjector?tqaCustomize=true&injectMode=public&date=MM/dd/yyyy&injectedUser=userId&publicCalendarName=calendarName
				2.4.Inject public events, tasks in public calendars 
						AND 
					private events, tasks into default private calendar:
				host:port/rest/bench/inject/CalendarDataInjector?tqaCustomize=true&injectMode=both&date=MM/dd/yyyy&injectedUser=userId&publicCalendarName=calendarName
				
				In 2.3 and 2.4: if the publicCalendarName does not exist, it will be created.	