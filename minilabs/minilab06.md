# Minilab 06

In project1, we looked at the most common
words in ratings with both 5 stars and 1 star. 
What if we needed to repeat this process regularly
for some other potential set of ratings?

Today we are going to adapt project 1 to accomplish
this by turning it into a shell script. 
If you didn't finish project1 or don't feel like
working with the whole list of commands, don't worry about
outputting the most common words, just create
your script so it goes as far as 
combining the relevant ratings into a file.

### Task
Write a shell script that
1. Takes as its first argument the path to the reviews directory
   (so it doesn't need to be inside the folder to run your script)
2. Takes as its second argument the rating number to
   process and output common words for that rating
   (or simply concatenate all reviews with that rating to
   a single file if you didn't finish the project).
   * Have your script check to make sure it is a valid rating number
     (so what happens if someone types in 0, 10, etc.)

### Hints
To accomplish this, you'll need to:
1. Create a shell script
2. In the script, use cd to change into the directory
   passed as an argument
4. Modify your cat command to use the inputted rating number.
5. If you finished the project, combine this and all of
   your commands into a script (hint -- commands.txt was
   basically a script just with a different extension).


### More Practice (Not Required)
If you want more practice, you could make other modifications
such as (not required for the minilab):
* Instead of accepting 2 arguments, loop through all possible
  values and produce output for all possible rating numbers
* Accept either 2 or 3 arguments.  If there are 3 instead
  of 2, use those as start/end for the range of ratings to
  process together as one.
