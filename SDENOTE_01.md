# SDE-NOTE 01

There is a difference between the current git version 
(git version 2.43.0.windows.1)
and the version used in the course.

In the latest version:
- to remove changes to the file from the staging area (but not from the w/d) we use:
	$ git restore --staged FILENAME
- to remove changes to the file from the working directory (complete removal) we use:
	$ git restore FILENAME

This is more elegant and consistent than the old way of doing it:
	$ git reset HEAD FILENAME
	$ git checkout -- FILENAME