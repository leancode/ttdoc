
# Quick Tutorials
* **How To Create New Permission.**
  1. Open PermissionFactory.class.php
  2. Search For "hr_report" You Will See How Permission Hardcoded
  3. Create Your Own Permission The Same way That "hr_report" Does



# Server Side
* Notes: You Can Create Permission Instance Using new Permission(), if you are inside interface it will automatically defined as "$permission" Variable. 

- **Permission->Check($Section, $PermissionName)**:
   Will Return True If User Has the Permission , False if Not 
   * Section = Permssion Section Name Like "hr_report", "your_section"
   * PermissionName = Comoonly It Will Be (view, edit, view_own, edit_own) but you can Custmize it (see the Quick Tutorials) 

- **Permission->isOwner( $ObjectCreatedBy, $UserID )** : 
  This Will Check If A User Is The Owner, It's Very Important To Check That When you Need to Allow "edit_own" For Example.
  * $ObjectCreatedBy = Pass the Object Created_by (Get If From It's Database Using Factory for Example) 
   **UserListFactory->getCurrent()->getCreatedBy()** This will Get User Created By
  * $UserID = Pass The User Id , You Can Get The Current UserId By Using 
    **UserListFactory->getCurrent()->getID()**

# Client Side

- **PermissionManager.validate(section, name) ** : 
  Will Return False Or True Based on User Premission

- **PermissionManager.checkTopLevelPermission( SectionName )**
  This will check Permission, But Not One Permission
  For Example: You Use This Methods When You Want To Show a tab or page For Admins, 
  But You Also Want To Show it For Normal Users, And Some Other Roles if they have The Permission.
  So You Should Create New Case Before Using This Methods. 
  Go To "PermissionManager.js -> checkTopLevelPermission" Search For "case 'Request'"
  And Create Your Own Case Based on It 