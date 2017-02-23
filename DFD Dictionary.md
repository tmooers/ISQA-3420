Entities: 
  - Developer: user who uploads software packages to be scanned and added to the OSS Package Database
  - Manager: user who can query open source software package database and create/edit/view policy

Processes: 
  - Check for OSS Components: Receives and distributes software package from developer to Scanner and NIST Vulnerability Database.
    Formats and stores software results in OSS Package Database
  - Scanner: scans software package and returns licensing results
  - Query Package: Receives query information from manager/developer and retrieves requested information from the OSS Package Database
  - Retrieve Policy: Receives policy request from manager and retrieves requested information from policy database
  - Edit Policy: Receives edited policy from manager and stores it in policy database
  - Create Policy: Receives new policy from manager and stores it in policy database

Databases: 
  - NIST Vulnerability Database: external database with known software vulnerabilities
  - OSS Package Database: internal database of licensing and vulnerability information of software packages
  - Policy Database: internal database of company policy on software

Data Flows: 
  - Software Package: package of software being sent from developer to be checked for OSS components
  - Software Results: results including license and vulnerability information
  - Package Name: name of software package used to check for vulnerabilities
  - Vulnerability Results: results containing vulnerability information about software package
  - Scan Results: results containing licensing information about software package
  - Info Query: request for information regarding a software package stored in the OSS Package Database
  - Query Results: results including information for a specific query
  - Policy Request: request for information regarding current policy
  - Policy: current company policy
  - Edited Policy: updated policy information to be stored in policy database
  - New Policy: new policy information to be stored in policy database
