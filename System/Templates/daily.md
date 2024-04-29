---
creation date: <% tp.file.creation_date() %>
tags: daily_note <% tp.file.title.split('-')[0] %>
type: daily_note
---
# <% tp.file.title %>
<< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]] | [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>]]>>

# New Today
 - 7:00 - 9:25 (DO):
	 - Review of activities from the previous week, planning activities for the day.
 - 09:25 - 11:51 (RE)
	 - Start of daily activities, work on main projects.
 - 11:51 - 14:16 (MI)
	 - Peak energy time, important meetings and discussions.
 - 14:16 - 16:41 (FA)
	 - Lunch break and reflection on activities done so far.
 - 16:41 - 19:07 (SOL)
	 - Continuation of main activities, focus on more challenging tasks.
 - 19:07 - 21:32 (LA):
	 - End of activities, time to relax and engage in hobbies or recreational activities.
 - 21:32 - 7:00 (SI):
	 - Free time for oneself, preparation for sleep.
 

#### Over Due
```tasks

not done

due before <% tp.file.title %>

```

#### Due Today
```tasks

not done

due on <% tp.file.title %>

path does not include Templates

```





## Meeting Log

```dataview
table start_time as "Start Time", end_time as "End Time", duration as "Duration" from "Meetings"
where date(date) = date(<% tp.file.title %>)
```
## Daily Log

### General

<% tp.file.cursor() %>

### Other




## Other Tasks

#### No Due Date
```tasks

not done
no due date
path does not include System

```

#### Done Today

```tasks

done on <% tp.file.title %>

path does not include System

```
