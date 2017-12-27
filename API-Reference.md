

- $this->returnHandler( $retarr ) 
  This Will Build The Structure For Your Returned Data
* Use $this->returnHandler( TRUE )  If There Are No Records From Db 
* $retarr = All Records That You Get From DB 


- $this->getPermissionObject()->Check($SectionName, $PermissionName)
  This Will Check if User Has The Specific Permission Return True Or False
 
- $this->initializeFilterAndPager( $data, $disable_paging ) 
  This Will Prepare Pagination and Filters And Use the Default Value if no provided from The Client

* $data = The Data Come From View

- TTnew($ClassName)
  This Will Create Instance Of The Class, But With It's Plugins
  So Make Sure You Use It To Let Other People Can Write Plugins For Your Main Class.

