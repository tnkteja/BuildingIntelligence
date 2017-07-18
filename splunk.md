# Splunk

I spun the splunk from docker using [1]. The challenge was when setting up the HTTP Event collector. I followed the steps on 
[2]. Yet the splunk wont seem to receive the logging messages though its HTTP Event Collector. [3][4] gives some lead on solving
it. While the port is unreachable, there is no firewall setup on the machine. So the docker had to be checked to see it has a 
binding to 8088 port though container to the docker machine.

## References
1. _https://hub.docker.com/r/splunk/splunk/_
2. _http://dev.splunk.com/view/event-collector/SP-CAAAE7F_
3. _https://answers.splunk.com/answers/508322/splunk-db-connect-3-how-to-find-out-if-the-http-ev.html_
4. _http://dev.splunk.com/view/csharp-sdk-pcl/SP-CAAAE7W_
