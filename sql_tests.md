# SQL Queries tests, results, answers

## The queries

For each of the questions below, add the following information to a Markdown file in your homework repo:

* Find all time entries.
    * SELECT * FROM time_entries;
    * 500 rows returned
* Find the developer who joined most recently.
    * SELECT * FROM developers ORDER BY joined_on DESC LIMIT 1;
    * "34"	"Dr. Danielle McLaughlin"	"shakira.carter@kohler.org"	"2015-07-10"	"2015-07-14 16:15:19.224045"	"2015-07-14 16:15:19.224045"
* Find the number of projects for each client.
    * SELECT *, COUNT(projects.id) AS num_of_projects FROM clients LEFT JOIN projects ON clients.id = projects.client_id GROUP BY clients.id;
    * 12 rows returned. 
        * NOTE: I originally started using JOIN, but then thought I should use LEFT JOIN to show clients who have no projects. For some reason, though, it took me a while to figure out to count projects.id not clients.id.
* Find all time entries, and show each one's client name next to it.
    * 
    * 
* Find all developers in the "Ohio sheep" group.
    * 
    * 
* Find the total number of hours worked for each client.
    * 
    * 
* Find the client for whom Mrs. Lupe Schowalter (the developer) has worked the greatest number of hours.
    * 
    * 
* List all client names with their project names (multiple rows for one client is fine).  Make sure that clients still show up even if they have no projects.
    * 
    * 
* Find all developers who have written no comments.
    * 
    * 

Unless otherwise specified, return all columns in the requested table (e.g. developers).

## Challenges

Try these queries if you have time:

* Find all developers with at least five comments.
    *
    *
* Find the developer who worked the fewest hours in January of 2015.
    *
    *
* Find all time entries which were created by developers who were not assigned to that time entry's project.
    *
    *
* Find all developers with no time put towards at least one of their assigned projects.
    *
    *
* Find all pairs of developers who are in two or more different groups together.
    *
    *
