---
type: daily
---

[[Journal/<% tp.date.now("YYYY-MM-DD",-1,tp.file.title,"YYYY-MM-DD") %>|Yesterday]] <== [[<% tp.date.now("YYYY-MM-DD",0,tp.file.title,"YYYY-MM-DD") %>]] ==>[[Journal/<% tp.date.now("YYYY-MM-DD",+1,tp.file.title,"YYYY-MM-DD") %>|Tomorrow]]


# Tasks for the Day

fill by hand


# Queried Tasks Due Today

```dataviewjs
dv.taskList(
  dv.pages().file.tasks
  .where(t => t.text.includes("{{date:YYYY-MM-DD}}"))
)
```



# Journaling

