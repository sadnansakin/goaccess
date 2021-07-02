# goaccess 🔥🔥
## SADNAN 🔥

My Source: https://github.com/sadnansakin/goaccess/blob/6a823d4d26686b56291ef8a0547bd9d23c492689/working_commands.md

### Very Basic
goaccess access_log_collected.log

### interactive html report with Dashboard ->
goaccess access_log_collected.log -o access_log_report.html --log-format=COMBINED

### filtering , piping and adding result to the html report ->
cat access_log_collected.log | grep '200' | goaccess -o access_log_report200.html --log-format=COMBINED -

### very specific filtering then pipe it to (goaccess) ->
cat access_log_collected.log | grep '20/Dec/2020:05:30:' | grep 'POST' | goaccess --log-format=COMBINED
