---
ID: 2587
post_title: Version 0.0.2 of WP-Gitdown Published
author: James DiGioia
post_date: 2014-02-20 18:14:44
post_excerpt: ""
layout: post
permalink: >
  http://jamesdigioia.com/version-0-0-2-wp-gitdown-published/
published: true
---
I've uploaded the next version of [WP-Gitdown to GitHub][1], which is just two improvements:

*   I completed a feature that will publish, update, and delete posts as you write, and push all the changes to your public repo
*   Some minor bugfixes and improvements on the back-end of the code

The next big part is pretty much going to be the core of the plugin: pulling from the remote repo and loading any changes content from the files into the database. Writing the trigger shouldn't be too hard.

1.  Run `git pull`
2.  Check for changes between the file and the database
3.  If there are changes, update the database

The question is when is the trigger going to fire. My first inclination was when you open the post in the editor. The problem with that is if a change is made via pull request/editing in the repo itself, the changes won't be reflected on the site until someone goes into the post itself and updates it, which is an extra step I'd like to avoid.

In any case that's where I'm at. I think version 0.1 will be next - it will be the "feature complete" version that gets all the basics in there, then bug fixes until it's stable enough to be version 1.0!

 [1]: https://github.com/mAAdhaTTah/WP-Gitdown