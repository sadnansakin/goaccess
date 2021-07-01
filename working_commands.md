## Very Basic  
goaccess access_log_collected.log 

## interactive html report with Dashboard ->
goaccess access_log_collected.log -o access_log_report.html --log-format=COMBINED

### filtering , piping and adding result to the html report ->
cat access_log_collected.log | grep '200' |  goaccess -o access_log_report200.html - 
