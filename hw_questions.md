# SQL Homework Questions

Use the supplied data as the source of data to answer the questions.  Copy the SQL command you have used to get the answer, and paste it below the question, along with the result they gave.

## Questions

1. Return ALL the data in the 'movies' table.
select * from movies;

2. Return ONLY the name column from the 'people' table
select name from people;

3.Oops! Someone at CodeClan spelled John's name wrong! Change it to reflect the proper spelling (change 'jhn Harper' to 'John Harper').
update people set name = 'John Harper' where name = 'jhn Harper';

4. Return ONLY your name from the 'people' table.
select name from people where name = 'Allegra Perazzo';

5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
delete from movies where title = 'Batman Begins';

6. Create a new entry in the 'people' table with the name of one of the other instructors (Tony, Kat, etc).
insert into people (name) values ('Tony Gonzo');

7. Zsolt, has decided to hijack our movie evening, Boo! Remove him from the table of people.
delete from people where name = 'Zsolt Podoba-Szalai';

8. Somehow the list of people includes two people named 'instructor'. Change these entries to the proper names ('Darren Breen', 'Sandy McMillan')
update people set name = 'Darren Breen' where id = 10;
update people set name = 'Sandy McMillan' where id = 11;

9. The cinema has just heard that they will be holding an exclusive midnight showing of 'Guardians of the Galaxy 2'!! Create a new entry in the 'movies' table to reflect this.
insert into movies (title, year, show_time) values ('Guardians of the Galaxy 2', 2017, '00:00');

10. The cinema would also like to make the Guardian movies a back to back feature. Update the 'Guardians of the Galaxy' show time from 12:10 to 21:30
update movies set show_time = '21:30' where title = 'Guardians of the Galaxy';

## Extension

1. Research how to delete multiple entries from your table in a single command.
