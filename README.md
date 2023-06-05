# jmeter
jmeter stuff 


Script can be started from command line using 
jmeter -Jthreads=2 -n -t grafana.jmx 

results will be stored in grafana_aggregate.xml -file.

List_A.csv contains list of Views that script will go thru. 
modifying that will affect what views script will go thru.

example starting from command prompt, log file defined also.
jmeter.bat -n -t grafana.jmx -Jthreads=2 -j grafana_log.xml


Test path
1. main page with default view
2. change view based on List_A.csv value, last 30 min
3. change view based on List_A.csv value, last 60 min
repeat until view contains no data
4. use same time frame, but 6 days (or 4,5 days) in past, no weekend days
when no data, consider it as error and start thread from beginning, using next value from List_A

test duration 600 sec