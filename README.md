# Ephorus Assignment
This building block provides an Ephorus integration with Blackboard. Instructors can create specific Ephorus assignments in their courses, for which all submitted work will be scanned by Ephorus for plagiarism.

To use this building block you need a contract with Ephorus (now owned by Turnitin). Please contact 
Turnitin Ephorus Support <ephorussupport@turnitin.com> for any questions regarding this building block.

## Links
- [Download Latest Release](https://github.com/rijksuniversiteit-groningen/b2-EphorusAssignment/releases/latest)
- [View All Releases](https://github.com/rijksuniversiteit-groningen/b2-EphorusAssignment/releases)

## Release Notes

### 3400.190919.0
- Removed the filter on invalid XML characters for the incoming reports. This fixes that a report will not show Microsoft quotation marks, but there is a risk that a report will not be accepted; keep an eye on the "list missing reports" page found on the main Ephorus configuration page.

### 3400.190726.0
- compatible with Blackboard release 2018 Q4 ("3500.0.x"), older versions of the b2 give 'RuntimePermission" "createSecurityManager"' and 'unsupported connection class: blackboard.db.impl.SafetyNetConnection' errorsin the logs
- fixed exception when a group assignment is already submitted but student is also in another group that is unavailable
- when a course gets deleted all the Ephorus data (assignments, documents, reports) will also be removed from the Ephorus database

### 3400.181115.0
- compatible with Blackboard release 2018 Q2 ("3400.0.x"), older versions of the building block will _not_ work correctly in this Blackboard version
- fixed error when someone is using the cross-course navigation 
- option to use logging in a format that Blackboard SAAS expects
- option (experimental) to send logging to an ElasticSearch server
- new privilege "Resubmit documents to refresh their plagiarism report" which gives a "resubmit" button in the assignment document list; by default only visible to system administrators

### 3200.180321.0

- in Blackboard 2017Q4 adding an attachment to an Ephorus assignment gave an error

#### Supported Blackboard versions
Q2 2017-Q4 2017


### 3000.171006.0

- rework function was broken in version 3000.170822.0 

#### Supported Blackboard versions
Q2 2016-Q2 2017

### 3000.170822.0

- Now compatible with the LIS data integration building blocks.
- Students can now download feedback that has a "+" in its filename.
- Fixed the "Change Status" buttons in My Documents.
- Display a message when Blackboard cannot send the e-mail from the rework submission page.

#### Supported Blackboard versions
Q2 2016-Q2 2017

### 3000.170411

- Fix for 'missing vital information' when viewing a report for an instructor upload.
- Prevent JavaScript exception in listDocuments for individual assignments.

#### Supported Blackboard versions
Q2 2016-Q2 2017
