---
company: Dr.M Inc
location: Libanon
title: King Of The Hill
email: mb@mahmoudb.com
phone: 
aliases:
  - MB
task_tag: drm
type: person
---
# [[Dr.M]]

## Meetings
```dataview
TABLE summary as "Summary" from [[Dr.M]]
where contains(type,"meeting")
sort date desc
```
## Pending Tasks
```tasks
tags include #dr.m
path does not include System
```

## Completed Tasks
```tasks
done
tags include #dr.m
path does not include System
```