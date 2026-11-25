# Question 10: Scholarship Application Assessment

PostgreSQL. Run `solution.sql` from top to bottom. It creates its own schema `q10`.
Scheduled jobs use pg_cron.

## Index
`applications(status, submitted_on)`

The search filters on one status (equality) and a submitted_on range. status first, submitted_on second lets PostgreSQL read just the matching status and date window from the index.
