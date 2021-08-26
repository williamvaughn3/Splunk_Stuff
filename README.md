# Splunk_Stuff

Install the spl Bastogne App	***see notes at the end of this file for name change instructions***
Create Username bctcyber
Create bctcyber user, needs at min. power and admin rights, but I gave all the base. 
(not required, but the owner is specified as bctcyber, you can reassign knowledge objects if desired instead)

Click App Manage Apps
	Install from file
	Install the Bastogne.spl

Install the Dependencies.
	-> link-analysis-app-for-splunk_161.tgz
	-> splunk-add-on-for-microsoft-sysmon_1062.tgz
	-> force-directed-app-for-splunk_301.tgz
	-> timeline-custom-visualization_140.tgz
	-> lookup-file-editor_333.tgz
	-> sankey-diagram-custom-visualization_140.tgz
	-> sideview-utils-free-internal-use-license_3410.tgz
	-> Punchcard app 

Hide non-necessary apps and keep from checking for updates from the menu
	-> Manage Apps again
	-> click edit properties
	-> radio buttons for the check for updates and view in menu are unselected and selected as applicable.

The app is installed.

You can go to the lookups to create your whitelist, and specify the internal IPs.





***
The apps.conf file on the splunk vm will allow you to change the display name via command line.  

***
 I used 'infosec-indexes' from another applicaton for some searches. 
 It is set to index=*, which looks at all indexes.  For many of the search strings, you can just substite infosec-indexes with the value,
 but using macros will greatly allow for tuning and centralized control in the future.  
 If you change, add, remove, or update sourcetypes, want to filter further, updating a macro is more manageable.  Otherwise you would have to update each
 query in the all dashboards.  Wish this was realized earlier in the build.
 
