# Splunk_Stuff
>
The dependencies are listed below. The app was created by aggregating multiple apps' logic and tweaking the dashboards.  Love splunk because it so easily allows you to stand on the shoulders of Giants and call yourself tall.  The Splunkbase is such a good resource to turn your data into information.  
> 
This was a fun project that nobody cared about until the recent class just used it.  It was very awesome seeing it being leveraged, but also leveraged correctly.  Turning data into information is cool, but it doesn't become knowledge until leveraged and shared. 
> 
So special thanks to Kevin and his class for the humbling experience to see some bad ass professionals do some bad ass Defending and the two way street of building knowledge.

Install the spl Bastogne App	
(AND CHANGE THE NAME-I was Drinking the Orgs Kool-Aide when I named it)


Click App Manage Apps
>
> Install from file
> 
> Install the Bastogne.spl

Install the Dependencies.
>
> link-analysis-app-for-splunk_161.tgz
> 
> splunk-add-on-for-microsoft-sysmon_1062.tgz
> 
> force-directed-app-for-splunk_301.tgz
> 
> timeline-custom-visualization_140.tgz
> 
> lookup-file-editor_333.tgz
> 
> sankey-diagram-custom-visualization_140.tgz
> 
> sideview-utils-free-internal-use-license_3410.tgz
> 
> Punchcard app 

Hide non-necessary apps and keep from checking for updates from the menu
> 
> Manage Apps again
> 
> click edit properties
> 
> radio buttons for the check for updates and view in menu are unselected and selected as applicable.


I used 'infosec-indexes' from another applicaton for some searches. 
 It is set to index=*, which looks at all indexes.  For many of the search strings, you can just substite infosec-indexes with the value, but using macros will greatly allow for tuning and centralized control in the future.  

You can go to the lookups to create your whitelist, and specify the internal IPs, also you'll want to create a macro for the infosec-indexes that contain the indexes for your 

If you change, add, remove, or update sourcetypes, want to filter further, updating a macro is more manageable.  Otherwise you would have to update each  query in the all dashboards.  Wish this was realized earlier in the build.  But I was learning as I was building it
 
