## CONGRESSIONAL APP 2026 SUBMISSION

https://comp-fvhs.vercel.app/

tracking community service hours has always been the greatest pain. in fact, I just fell for a fake captcha which led me to install malware, because our school's Baron News website was compromised. the official FVHS spreadsheet for tracking hours for the 160-hour community service cord isn't on the official FVHS website; it was linked in a Baron News article that, almost got me a virus. and that "spreadsheet" is rather a table function on a google doc. logs aren't organized; you spend way too long scrolling through your photo album and looking through photo metadata for dates and locations, and try to remember the events you didn't take pictures of, just to end up with a jumbled mess on a doc.

## not another productivity app

the app was made for and built by 4 seniors in high school; it was meant to solve issues we encountered over a shared 4-year experience, and to build the "what would I wish I had as a freshman..." thought.

note: some might not have been implemented yet; we didn't get around to some before the congressional app deadline and didn't want to push any new code past the deadline, in case that might have disqualified us.

## added features

1. connects clubs & their volunteer events to students
  - club rush happens for two lunches at the beginning of each semester, then never again. the typical student joins one or two clubs, and misses all of the opportunities the other 80 provide. comp will create a space not only for club leaders to promote their events, resulting in higher yields, but also a space for students to find those opportunities to begin with. students aiming to clear their 160 hours in a shorter amount of time, or students who want to find a greater range of volunteering events stand to benefit.
2. logs hours & events in one place
  - a spreadsheet is a pain to update and a pain to keep organized. one column for how many hours you where there, another describing the event, another for the club, and no space for a group picture. comp is like Instagram; every event attended is logged with hours, approval from a supervisor (if needed), and a picture to affirm and commemorate the event. if comp starts to gain traction post congressional app judgment, we could easily add an Instagram-like "feed" page for students to share their good deeds
3. opportunity sniffer
  - scholarships & extracurricular opportunities are CRUCIAL for students to be applying for throughout high school. comp has a page dedicated to connecting students to scholarship & non-volunteer extracurricular opportunities. devs and club leaders are also free to post on this page. (a good example would be stardance by hack club.) 
4. college application hub
  - fafsa, transcripts, letters of recs, activities list, piqs, common app essays; multiple aspects of a college application that take 25 tabs and 64 gb of ram to manage. it's multiple different application websites and a million things to keep track of. comp keeps it all in one place, with a timeline feature to keep you on track.
5. study resources
  - free study resources (practice problems, videos, etc.) for every stem ap class & exams like the SAT

## features we didn't get around to before the deadline

6. social media for clubs
  - club-to-club collaboration is rare and typically happens between friends. social media is informal and hard to manage between groups. comp could creates that space for club leaders to connect, either through direct messaging between club leaders and/or club comp accounts
7. club tracking
  - similar to volunteer hours, club leaders may find tracking membership and participation equally tedious and chaotic. comp could create one event, and every comp member who claims that event is automatically tracked, able to be managed by the club leader. one feature comp already incorporates is that accounts can be associated with a school. clicking on that school's tab shows all students registered into comp at that school; a similar feature for clubs could easily be added. this feature could also be used to track participation from member to member, and to create a member leaderboard within clubs, and a club leaderboard between clubs. (ranked on volunteer hours, member count, etc.) this leaderboard is already a feature within comp.

##  LIVE DEPLOYMENT AT: [https://winterrmelonn.github.io/comp/](https://comp-fvhs.vercel.app/)

## Run

No build step. Serve the folder (e.g. `python3 -m http.server 8123`) and open http://localhost:8123.

Accounts, hours, clubs and posts live in Supabase (project URL and publishable key in `db.js`). To set up a fresh project, run the `supabase*.sql` files in order (`supabase.sql`, then `supabase-2.sql` … `supabase-14.sql`) in Supabase → SQL Editor.

Guests can still log hours without an account; those stay in the browser's localStorage and can be moved into an account from the profile page. **Download CSV** gives you a backup.

## Test

```
node test.js
```
