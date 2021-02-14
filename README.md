# Power BI Log Analytics 

<img src="https://images.squarespace-cdn.com/content/v1/57aa0fb1b3db2bbe2dfb5840/1607362034987-W2CCN0CV3112IH7MO9PP/ke17ZwdGBToddI8pDm48kHetbtA8IrNNARGRRAMq6VBZw-zPPgdn4jUwVcJE1ZvWEtT5uBSRWt4vQZAgTJucoTqqXjS3CfNDSuuf31e0tVHhoieEUztzpJSjZ_qXSmFcXEpZNATOgXau2Y02sfc7AN1lH3P2bFZvTItROhWrBJ0/Power+BI+Logo.png" align="right"
     alt="Power BI Logo" width="120" height="178">

Power BI Log Analytics is a free tool, helping you to fetch the right insigth about your Power BI usage. This is a starter kit giving you a vision on what you can do and what
kind of data you can have.

As you can see, i used PowerShell to extract the data and save files in my local computer. You can tweak the shell to save the data into Azure Datalake. I also used my username,
you can use Service Principal for more security. I did it easy way to go fast :).

# Prerequisites

* PowerShell V7.0
* Power BI Administrator role

# Limitations

* The API call (`GetGroupsAsAdmin`) you must specicy a limitation parametre (`$top={$top}`) and the limitation is 5000. In case you have more than 5K Workspaces you'll be stuck ! in case you have several Premium capacity, then you can filter per capacity. So, lucky you are:).
* The API call (`Refreshables`) wil fetch only the data about the last refresh. In case your dataset refreshing several times per day, you'll get only the last status.
* There is an API (`Get Refresh History`) allows you to get the history refresh. But, you need to be part of each workspace.

# Versions
* 1.0.1 : Addinf new KPI in (`Refresh Schedule`) "Ratio Dataset Activity / Refreshs" giving you the balance between the usage of the dataset versus the refresh
* 1.0.0 : 

# Documentations
     
### Activity
- Activity by user :
- Activity by Category : 
- Activity by Domain : 
- Activity by Capacity : 
- Activity By Date : 

### User Activities
- User per Workspace : 
- Activity per users
- User by domain : 
- User by Capacity : 
- User By Date : 

### Activities details
- Activity matrice details : 

### Inventory & Roles
- Inventory by Capacity, Worksapce, User & Access Right : 
- Users by Access Right repartition : 
- Users by Capacity Name and Access Right : 

### Workspaces Details
- Inventory by Capacity, Worksapce, User & Access Right : 
- Inventory by Capacity, Worksapce, User & Access Right : 

### Inventory Evolution
- User per Workspace : 
- Activity per users
- User by domain : 
- User by Capacity : 
- User By Date : 

### Refresh Schedule
- User per Workspace : 
- Activity per users
- User by domain : 
- User by Capacity : 
- User By Date : 

### Refresh Status
- User per Workspace : 
- Activity per users
- User by domain : 
- User by Capacity : 
- User By Date : 

### Gateways
- User per Workspace : 
- Activity per users
- User by domain : 
- User by Capacity : 
- User By Date : 

### Datasources
- User per Workspace : 
- Activity per users
- User by domain : 
- User by Capacity : 
- User By Date : 
