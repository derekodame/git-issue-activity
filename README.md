# GitIssueActivity
Activity for practicing with git and issues on GitHub.

For this activity, the students will practice making changes to a GitHub repository. 
The repository has a text file that has been "scrambled" - meaning that random words
have had their characters randomly rearranged, and considered to be issues to be fixed.

The students will:

1. Fork the repository
2. Clone the repository
3. Add the original repository as an upstream remote:
	
	`git remote add upstream git@github.com:CS-Worcester-CS-348-SP-2018/git-issue-activity.git`
4. Create a `fix-license-typos` branch, and switch to that branch:

	`git checkout -b fix-license-typos` 
5. Repeat as often as possible during the class:
	1. Assign themselves to an issue on GitHub (e.g. issue #42)
	2. Edit the LICENSE.txt file to correct the issue
	3. Add the change
	4. Pull any changes that have ocurred since their last pull, and correct merge conflicts
	4. Commit the change, with a message describing the change (include line number and correction, e.g. `Correct misspelling, line 1: UGN -> GNU` )
	5. Push the change

	`git push upstream master`
	6. Make a pull request to have their change merged into the original repository, including in the pull request text a notation that it closes the assigned issue (e.g. `Closes #42`)

The misspellings were generated by the `twiddle.py` program and then entered as issues by the `report.py` program (from this [git-twiddler fork](https://github.com/kwurst/git-twiddler).