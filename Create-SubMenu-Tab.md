
Search for "TopMenuManager.js"

And Search For "TopMenuManager.buildRibbonMenuModels" Function
Just Copy Paste Any SubMenu Item You Want to Make It Like It.
For Example


`var request = new RibbonSubMenu( {
		label: $.i18n._( 'Requests' ),
		id: 'Request',
		group: myAccountGroup,
		icon: 'requests-35x35.png',
		permission_result: PermissionManager.checkTopLevelPermission( 'Request' ),
		permission: permission.request
	} );`

if you duplicate This You Will See New Item Inside "MyAccount" 
And Edit The Option As You Like.

Options: 

**label** = The Tab Name 

**id** = 

**group** = The Parent Tab Name 

**permission_result** = 

**permission** = 