
This Quick Guide Will Teach You How To Add New Tab to existing window 

1. Open "EmployeeViewController.js"
2. Search For "tab_audit" inside "setTabStatus" function Take A look How They Check Permissions 
   And How They Decide To Show Or hide
3. Duplicate "tab_audit" change it for anything you like, for example, "docs"
   also, give another attr "ref" for it for example "tab_documents"

4. Search For "tab_audit" Inside "buildEditViewUI" function
   See How They Order Thier Tab. Add Yours At The End With The same "ref" that you create in "3." 

5. Open "EmployeeEditView.html"
6. Search for "tab_audit" in file, You will Find More Than One Results. check them 
7. Duplicate They Information You Found, and change the Information To Match The Info You had Write in "EmployeeViewController.js" 
