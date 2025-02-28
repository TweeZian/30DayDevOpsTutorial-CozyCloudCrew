Day 3 | DevOpsAllStarsChallenge

Using
S3
Glue
Athena

Took code from github
changed region to Singapore
changed bucket name to add random

Cloudshell in AWS
create setup.py, env and delete.py files
paste codes
check if pip has dotenv installed, if not use pip install python-dotenv
put API and endpoint into .env
run setup
check and test
run delete file
check AWS console to see if delete is successful

Athena
From here, can run sample query

SELECT FirstName, LastName, Position, Team
FROM nba_players
WHERE Position = 'PG';

have to set saved query result to a location, use S3 created