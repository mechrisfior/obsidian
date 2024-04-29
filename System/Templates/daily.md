---
creation date: <% tp.file.creation_date() %>
tags: daily_note <% tp.file.title.split('-')[0] %>
type: daily_note
---
# <% tp.file.title %>
<< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]] | [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>]]>>

# #### New Today

## Tasks

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
