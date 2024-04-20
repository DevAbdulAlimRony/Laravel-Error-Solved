
## Laravel Error and Solution

This Readme provides the errors I fetched during doing my project and solutions.


## Migration: Cannot add foreign key constraint

- Problem
    - Everything was fine. My migration file already had proper foreign keys, but still occured the same error again and again. Well, after a long run, I have just figured out something. I made my parent model's migration after making the child model's migration.

- Solution
    - Don't make the child migration first. Make Parent Model's Migration, then go to the Child.
    - Ex. Profile belongs to a User. If you make Profile migration at first and then User migration, then you will get the error. Copy all migration's code, delete them, and again create the migrations- User and Profile respectively.

