# apigee-reports

# Summary
This repo documents how to create a custom proxy reuse report that shows all the proxy names and which developers/developer apps are consuming them.

# Create the Custom Report
1. Click Analytics then click Reports
![Analytics -> Reports](/images/analyticsreports.png?raw=true "Analytics Reports")

2. Enter the following and then save the report.
* Report Name : ProxyReuse
* Select `Traffic` as the `Metric`
* Select the following `Dimensions`
  * `Proxy`
  * `Developer Email`
  * `Developer App`

![Custom Report Config](/images/customreportscreen.png?raw=true "Custom Report Screen")

3. Once you save the report, you will be able to see all proxies and the total number of requests sent to each one.

![Report View](/images/reportview.png?raw=true "Report View")

4. If you click on a proxy it will display all the developer email addresses that consume that proxy.  This assumes that the proxy includes either a Verify API Key or Validate Access Token policy, which identifies the developer.  

**Notice that this report does not display the developer email addresses.**

![Report View Developer Email](/images/reportviewdeveloperemail.png?raw=true "Report View Developer Email")

5. If you click on a Developer's email address, then it will list all the developer Apps that are consuming this proxy.  This also assumes that the proxy includes either a Verify API Key or Validate Access Token policy, which identifies the developer.  

![Report View Developer App](/images/reportviewdeveloperapp.png?raw=true "Report View Developer App")
