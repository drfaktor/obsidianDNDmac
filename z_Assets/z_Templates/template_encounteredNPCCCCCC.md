---
NoteType: encounterSheet
tags:
  - NPC
Gender: 
Race: 
Age: 
Class: 
Alignment: 
location: 
world: 
campaign: 
date:
  "{}":
---

> [!infobox]
> # `=this.file.name`
> ![[z_Attachments/placeholder.png]]
> [[z_Attachments/paceholder.png|Show To Players]]
> ###### Basic Information
> Type | Stat |
> ---|---|
> Home | `=this.Location` |
> Group | `=this.AssociatedGroup` |
> Sex | `=this.gender` |
> Race | `=this.race` |
> Age| `=this.age` |
> ﻿﻿Condition | Healthy |
> ###### Rules Info
> Type | Stat |
> ---|---|
> Alignment | `=this.alignment` |
> Class | `=this.class` |
> Character Role | `=this.character-role` |


```
<% tp.file.title %>
<% await tp.file.move("/2. Mechanics/Non-Player Characters/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewNPC");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter NPC Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>
```


```
# `=this.file.name`
```

### Appearance
<% tp.file.cursor() %>

### Motivation

	desribe motivation here

### Misc Info

	describe misc stuff

> [!info] Statblock
> ```statblock
> name: Individual
> monster: Commoner
> columns: 1
> ```


