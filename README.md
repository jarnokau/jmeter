# jmeter
jmeter stuff 


Script can be started from command line using 
jmeter -n -t grafana.jmx 

results will be stored in grafana_aggregate.xml -file.

List_A.csv contains list of Views that script will go thru. 
modifying that will affect what views script will go thru.
Result is stored in grafana_aggregate.xml

example starting from command prompt.
jmeter.bat -n -t grafana.jmx -JVUsers=2 -j grafana_log.xml