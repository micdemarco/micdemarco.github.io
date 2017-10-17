---
author: micdemarco
comments: true
date: 2017-10-08 13:00:10+00:00
layout: single
slug: migrating-google-accounts
title: Migrating google accounts
tags:
- google account
- drive
- photos
- keep
- maps
- calendar
- contacts
- email
- migrate
- starred locations
---

I have been on the google train for some time and most of my content is stored there.  Recently I decided to start using a new primary address.  

I attempted to move all my content across from the old address without any epic downloads and uploads.    This post describes the steps I took after some research, failure and persistence.  It is not perfect, but enough to move on.

# 1. Email - quite straightforward

1. From new account settings -> accounts and import -> add a mail account
2. Enter account POP details
3. Emails get imported.  Ability to send mail using both accounts

# 2. Contacts - easy import export of a small file

1. Go to contacts old version
2. From old account select all contacts -> export
3. From new account -> import contacts -> select file etc...
4. Switch back to the new version

# 3. Drive - easy change of ownership

Migrating google drive was easy with the following steps

1. Select all files from old account (CTRL+A)
2. Sharing -> add new account
3. Change access of new account to Owner
4. From new account select all
5. Remove old account

# 4. Photos - wierd migration

Migrating photos was tricky.  It was not possible to transfer the ownership of the files like Drive.  I managed to migrate the photos, but could not find any way of migrating albums.

1. Set image quality setting in the new account
2. From old account settings -> shared libraries -> share library with new account
3. From new account accept the invitation and add all the images to the library
4. From old account remove the library sharing

**Warning** *I tried deleting files from the old account and they still appear in the new account, however I am still not fully convinced the files now belong to the new account and haven't deleted the old files yet.  I will update after my old storage expires*

# 5. Keep - manual copy each note

I did not have too much content here, so I just opened 2 browsers side by side and copied away ... *sigh*

# 6. Maps Starred Locations - manual + painful

This was the biggest pain point.  I had over 500 starred locations to migrate.  It's possible to export the locations, create KML, and create a custom map (see [here](https://productforums.google.com/forum/#!msg/maps/Zp7LFnk5s3c/f3Ek6PxBk4kJ)), but this is not the same as having the nice stars overlayed on the map.

After some failed attempts to modify and replay http requests from the console, I gave up and tried to find an efficient manual approach.

1. Export locations from [https://www.google.com/bookmarks/](https://www.google.com/bookmarks/)
2. Split the file into separate files with 100 links per file
3. From chrome bookmark manager click organise -> import bookmarks from html file
4. Right click on the imported folder and Open all
5. Turn off your brain
6. Tab by tab click the star and close the tab with Ctrl-W.  The stars are mostly in the same place
7. Repeat

100 stars took about 5 minutes.  Total time to do everything about 1 hr.  

# Wrap up

Migrating google accounts is difficult and painful.  It is easy to extract your data using [Google takeout](https://takeout.google.com/settings/takeout), but it is not clear how to import this data back.  I'll be keen to hear about other cleaner / more efficient ways of doing this.