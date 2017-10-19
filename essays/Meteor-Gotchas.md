---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-10-19
labels:
  - Software Engineering
  - Meteor
---

To be entirely honest, my most time consuming issues in Meteor have been largely caused by simple errors in grammar, syntax, and formatting.

At one point, the app's stylesheet stopped loading altogether.  As far as I could tell, there were no problems with the code that imported the stylesheet, and it was targeting the proper elements.  The app worked perfectly fine except for the improper styling.

It turns out the problem has nothing to do with the stylesheet or the import statements for the stylesheet, rather, the problem existed in an entirely different file trying to import a page which did not exist.  I had initially disregarded the other import's error as irrelevant to my issue, something to fix later, however, somewhere in Meteor's compilers, this error blocked some of the later import statements.

If you have one issue that throws exceptions but has no apparent effect, and one which has noticable effect but no apparent source, fix the one you can find first, it may well be the root of the whole problem.

Later, when working on forms, I couldn't figure out why my form wouldn't submit.  The button showed up, the JavaScript was right, but it just wouldn't work.  The solution to this was far simpler, though it took an embarrassingly long time to spot, the "button" wasn't a button per se, but a div with the class button.

Lesson, things do what they say they do and not what they don't say they do.

But the main problem which has eaten the greatest amount of time has been simply naming things incorrectly.  Importing "contacts/contacts" and not "contacts/contacts.js", puting Template.Edit_Contact_Page.helpers() in home_page.js, looking for contactDataField 'Email' when the field is 'email'.
