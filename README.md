# AutoBookmark - Vanilla 2 Forum Plugin #

Vanilla Forums, as of 2.0.18.2, didn't automatically email users when a discussion they commented on was commented on by someone else.  I wanted that to happen, so I repurposed the bookmarks feature.

If you enable email notifications by default on bookmarked discussions by adding this next line to your config.php then unless a user changes their own preferences, they will be notified when a discussion is updated.

`$Configuration['Preferences']['Email']['BookmarkComment'] = '1';`


The Bookmarked Discussions module will show up in your sidebar and for active users it will probably become too long for your liking. Disable it by adding this line to your config:

`$Configuration['Vanilla']['Modules']['ShowBookmarkedModule'] = FALSE;`