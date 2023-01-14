# vintage-apple-II
Vintage projects for Apple II computers

WEEK.app

WEEK.app (Week In Advance) is an Applesoft Basic program I wrote in 1988 to track things I needed to schedule when I was in high school. The whole program functions in text mode, but I wrote it to mimic a graphical user interface re. icons and windows (it does not use a mouse, though). Functions are accessed through the keyboard, most with single-key inputs.

The main screen gives you 7 days in a week, in which you can place events. You press a number key from the main screen to carry out a function. After requesting to add events to a day, or view/edit a day's events, it asks you which day of the week you want. You put in a 3-letter abbreviation for the day (just as you see above each day "icon". Once you put that in, it opens a window on that day's events.

When it opens a window, it displays above the window the keys you can press to do something in the window and/or get back to the main screen.

If you select ADD EVENTS from the main screen, it doesn't display any events for the day you select, even if you've entered some. It's just a space to add events to that day.

Events are limited to two lines of text.

If you select VIEW/EDIT A DAY from the main screen, it displays any events you've entered for that day, allowing you to insert a new event, or edit, or delete any existing events in that day.

If there are more events than fit in the window, you can scroll the window to see more.

If you request to insert an event in this window, or to edit or delete an event, it will line up numbers along the left side of the window, allowing to apply the function you selected to a slot in the event list.

If you want to insert an event, it will ask where in the list you want to place your new event. The existing event you select, and any following it, will be moved down one place, after you enter the text for your new event in a subwindow it brings up. Note: The subwindow for this function just uses an Applesoft Input statement to capture the text you enter.

If you want to edit an event, it will ask you which event you want to edit. Once you've selected one, it will bring up a small subwindow with the requested event in it, with the cursor placed on the first character. Unlike the insert-event function, this subwindow does not use Applesoft's Input command for the input. From where the cursor sits, you can use the left and right arrow keys to move the cursor through the text of the event. You can replace characters by just typing over them.

The edit-event subwindow has an insert mode you can access by pressing Control-I. Once you enter this mode, every character you type moves the text to the right of the cursor to the right (it wraps the text, if necessary). You get out of this mode by either moving the cursor with a cursor key, or pressing Return (which saves your edited event).

The edit-event subwindow also has a delete-character function you access by pressing Control-D. Unlike insert mode, this is not a mode. It deletes one character at a time.

When you're done editing an event, you can press the Return key at any time, and all of the text in the subwindow will be saved back to the event you edited.

You can print a day's events from VIEW/EDIT A DAY by just pressing "P", once the window on a day has opened. For some reason I've forgotten, I only made the print function available in this mode.

Back at the main screen, it's also possible to clear a day's events in one step, by selecting CLEAR A DAY. You can also clear the entire week in one step, with CLEAR WEEK.

Once you're done entering or modifying a week's events, you can save the week to disk, using SAVE WEEK. It will ask you for a filename. Once you enter that, it will save the week's events.

Likewise, you can load a week's events, using LOAD WEEK.

Side note: One might wonder why I had two separate modes in which you can add events. A good question. ADD EVENTS was the first function I wrote in this application, and gradually realized I needed these other functions. However, ADD EVENTS allows one to quickly add multiple events to a day, without stopping. VIEW/EDIT allows you to enter one new event, if you want, after which, if you want to add more, you need to tell it you want to add another. A minor distinction. I probably could've done away with the ADD EVENTS function, but never did.

You can see a demonstration I made of Week In Advance in this YouTube video: https://youtu.be/LOF_49eomY0
