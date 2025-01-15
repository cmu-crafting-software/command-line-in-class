Excercises from https://swcarpentry.github.io/shell-novice/
1) You can also use two options at the same time. What does the command ls do when used with the -l option? What about if you use both the -l and the -h option? *Some of its output is about properties that we do not cover in this lesson (such as file permissions and ownership), but the rest should be useful nevertheless.*
2) By default, ls lists the contents of a directory in alphabetical order by name. The command ls -t lists items by time of last change instead of alphabetically. The command ls -r lists the contents of a directory in reverse order. Which file is displayed last when you combine the -t and -r options? **Hint:** You may need to use the -l option to see the last changed dates.
3) Starting from /Users/nelle/data, which of the following commands could Nelle use to navigate to her home directory, which is /Users/nelle?
    1. cd .
    2. cd /
    3. cd /home/nelle
    4. cd ../..
    5. cd ~
    6. cd home
    7. cd ~/data/..
    8. cd
    9. cd ..
4) Try the following command:
`$ touch my_file.txt`.
What did the touch command do? When you look at your current directory, does the file show up? Use `ls -l` to inspect the files. How large is `my_file.txt`? When might you want to create a file this way? To avoid confusion later on, we suggest removing the file you’ve just created before proceeding, otherwise future outputs may vary from those given in the lesson. To do this, use the following command: `rm my_file.txt`

5) When run in the alkanes directory, which ls command(s) will produce this output? `ethane.pdb methane.pdb`
    1. `ls *t*ane.pdb`
    2. `ls *t?ne.*`
    3. `ls *t??ne.pdb`
    4. `ls ethane.*`

6) We have seen the use of >, but there is a similar operator >> which works slightly differently. We’ll learn about the differences between these two operators by printing some strings. We can use the echo command to print strings e.g. running `echo The echo command prints text` will output `The echo command prints text`. If you run `echo hello > testfile01.txt` and then `echo world >> testfile01.txt` what is in `testfile01.txt`?

7) The `head` commandprints lines from the start of a file. `tail` is similar, but prints lines from the end of a file instead. Consider the file shell-lesson-data/exercise-data/animal-counts/animals.csv. After these commands, select the answer that corresponds to the file animals-subset.csv:
`head -n 3 animals.csv > animals-subset.csv` and `tail -n 2 animals.csv >> animals-subset.csv`. What is the content of `animal-subset.csv`?