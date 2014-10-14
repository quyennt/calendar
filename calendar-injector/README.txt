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
				host:port/rest/bench/inject/CalendarDataInjector?tqaCustomize=true&date=MM/dd/yyyy