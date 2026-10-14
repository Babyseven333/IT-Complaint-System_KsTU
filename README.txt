Adako Jachie Campus IT Complaint System (KsTU)
----------------------------------------------
1. Unzip this folder and double-click index.html to open it in a browser (no server, no database).
2. Normal users see only two tabs: Submit and Track.
3. The IT staff / Admin tab is visible to everyone but locked with a PIN. (Old note: it used to be hidden behind a double-click on the logo
   (or by adding #staff at the end of the page address), then enter the PIN.
4. Default PIN is 1234. Change it at the bottom of index.html: const PIN="1234"
5. In the IT staff tab, set each technician's name, phone and office, and the problem types they handle.

Data is saved in the browser of the device in use (localStorage).

Admin panel (inside the IT staff tab)
-------------------------------------
- Shows totals (Total, Open, In progress, Resolved) and complaints per problem type.
- New complaints show a NEW tag, an alert banner and "IT staff (n new)" on the tab.
- When a complaint is submitted, WhatsApp opens straight away to the assigned technician (if the browser blocks it, an "Alert <name> on WhatsApp" button shows in the pop-up).
  It opens WhatsApp to the phone number of the technician the complaint was assigned to.

Sound alert (new)
-----------------
- Voice alert, only inside the IT staff / Admin page after the PIN is entered: a short beep, then a voice says
  e.g. "You have 1 new complaint and 2 old complaints." It repeats every 12 seconds until you press "Mark all as seen".
  Normal users on the Submit and Track tabs never hear it.
- A new complaint submitted in another tab of the same browser also rings immediately.
- The browser tab title shows "(n) ..." for new complaints.
- Turn it off with the "Voice alert for new complaints" tick box.
- Note: browsers only allow sound after the admin has tapped/clicked once on the page (logging in with the PIN counts).
- Data is still stored per browser, so the admin must use the same device/browser that people submit on.
  For alerts from other phones/computers, use the WhatsApp alert button.

Files in this folder
--------------------
- index.html  : the whole system (code). The pictures are already built into it, so it works on its own.
- images/     : copies of the pictures (KsTU logo, WhatsApp icon) in case you need them separately.
