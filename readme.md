# News Log Analysis

This python script will hit a database, and answer a few questions we have already come up with.  The results are then output into a `news.log` file.

## Installation & Use

>> These instructions assume you already have a server or virtual machine running that you can use to execute python scripts against a PostgreSQL database:

- Load the data into the database by running `psql -d news -f newsdata.sql`
- Using the CLI, run `logviewer.py`

## Modification

If you would like to change the questions asked, you can do so by updating the `tasks` array within `logviewer.py.`  When supplying new tasks, you will need to supply 3 items:

1. A user-friendly question you need to answer (in plain English) 
2. A SQL query that works properly within the `news` database
3. A unit of measurement for the quantitative result that is provided