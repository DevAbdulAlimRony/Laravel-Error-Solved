
## Laravel Error and Solution

This Readme provides the errors I fetched during doing my project and solutions.


## Migration: Cannot add foreign key constraint

- Problem
    - Everything was fine. My migration file already had proper foreign keys, but still occured the same error again and again. Well, after a long run, I have just figured out something. I made my parent model after making the child model.

- Solution
    - Don't make the child model first. Make Parent Model, then go to the Child.
