## advance schemna patterns

| Pattern | Simple Goal | Real-life Analogy | 
|:---|:---|:---|
|Versioning | "Keep a history of changes. | "Microsoft Word " Track Changes | 
| Soft Delete | "Hide it instead of destroying it." | Computer Recycle Bin | 
| Audit Trail | "Record who did what." | A Security Camera / Logbook |

### 1. Versioning: "The Undo Button"
- Imagine you are writing a document. Instead of just saving over the old file, you save a new copy every time you make a major change (Version 1, Version 2, etc.).
- Why do it? If you make a mistake in the current version, you can go back and see exactly what it looked like yesterday.
- Simple Logic: Never delete the old data; just move it to a "History" folder so you have a timeline of how your data changed.

### 2. Soft Delete: "The Recycle Bin"
- In a normal database, if you hit "Delete," the data is gone forever (like hitting Shift + Delete on your computer). A "Soft Delete" is like moving that item to your computer's Recycle Bin.
- Why do it? It prevents accidental permanent loss. If a user deletes something by mistake, you can easily "restore" it later.
- Simple Logic: Instead of using the Delete command, you just add a label to the data that says isDeleted: true. Your app is then told to ignore anything with that label when it displays lists to the user.

### 3. Audit Trail: "The Security Camera"
- Think of this as a security camera recording who entered the room and what they touched. It doesn't necessarily stop the action, but it creates an unchangeable record of it.
- Why do it? If a record suddenly changes from "Price: $10" to "Price: $0," the Audit Trail tells you who changed it, when they did it, and what the price was before they touched it.
- Simple Logic: Every time someone makes a change, your system automatically writes a note in a separate "Logs" book. You never edit these notes; you just keep adding new ones to the end.
