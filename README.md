# IRS-MR-2019-01-19-IS1PT-IND-ZHAOYAZHI-Mortgage-Process
This individual assignment is based on the sample project Mortgage_Process in KIE workbench.

INSTALLATION & PREPARATION:
Please follow the steps below to prepare the system before you are able to use it.
  1.	Download the zip project file.
  2.	Extract the zip project file.
  3.	Open your KIE software and import the extracted project folder into KIE as a project
  4.	Ensure you have created these groups and assign some people to each group:
    a.	Iss-group-requester: iss-yazhi
    b.	Iss-group-manager: iss-sam
    c.	Iss-group-approver: iss-jack
  
ENHANCED FUNCTIONS:
The changes added is to have an additional check for supporting documents to determine whether applicant has submitted required documents. If required documents are not submitted, mortgage should not be issued.
  1.	Introducing a new field “Supporting Document” in Application data object.
  2.	Update forms with the new input field
  3.	Add checking supporting document as a new logic into existing Rules, and combine with existing rules table.

SAMPLE SCENARIOS & EMAMPLES:
  1.	Login as “iss-yazhi”, trigger instance and enter income as “110000”, property price as “250000”, property age as “3”, location as “Urban”, supporting document as “NRIC”, submit
  Login as “wbadmin” and go to inbox, “mortgage amount” should show as “200000”
  2.	Login as “iss-yazhi”, trigger instance and enter income as “110000”, property price as “250000”, property age as “3”, location as “Urban”, supporting document as “”, submit
  Login as “wbadmin” and go to inbox, no value will be set to mortgage.

