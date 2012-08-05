# oppo-time-tracker
============

A simple time-tracking app built with [Oppo](http://benekastah.github.com/oppo), a dialect of lisp that transpiles to javascript. It is a web app that runs on [node.js](https://nodejs.org). Both client-side and server-side javascript were generated through Oppo.

This app allows you to add projects and track how much time you have spent on them. It also allows you to track whether or not you have billed your client for time spent on a project and mark whether or not you have been paid for your work (for those of you who charge hourly). It groups time spent into two-week segments so it is easier to look at and work with It stores all this information in a sqlite database, which is automatically backed up every 24 hours.

This is a simple app, and one that I use every day. It demostrates how easy it is to create a web app in Oppo.

## To do

- Reorganize the routes. They have gotten pretty jumbled.
- Work on presentation so it is more friendly to read and use.
  - Make html and css DSLs in Oppo to this end. This would nicely demonstrate Oppo's excellent metaprogramming capabilities.
  - Make a prettier date and time presentation.
- Tweak database settings so it doesn't grow too large over time (I think it's the sqlite vacuum command I'm after, if I remember correctly).