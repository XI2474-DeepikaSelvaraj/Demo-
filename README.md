# API RESPONSE FOR GIS AND DMS
```http
GET /api/campaigns/?api_key=12345678901234567890123456789012
```


```javascript
{
  "message" : string,
  "success" : bool,
  "data"    : string
}
```

```http
1.{base url}/health
```
 ## successful Response:
    
    ```javascript
     {
      "status"
      "odbCount"
      "fiveGCount"
      "postGisVersion"
    }
   ```
```http    
2. {base url}/import/odb
```
   ## Request - Import the .kmz file
   ## Success Response:
   
   ```javascript
     {  "data":   
        "status": 
     }
   ```
      
     
   ## Failure Response:
     ```javascript
     {  "code": 
        "message": 
     }
     ```

3. {base url}/import/5g   
     Request - Import the .kmz file
    Success Response:
     {  "data":   
        "status": 
     }
     Failure Response:
     {  "code": 
        "message": 
     }
     --------
4.{base url}/odb/{yx}   
    Request :Input the lon and lat value separated by comma along with provider and type 
    Successful Response:
    {  "id": 
  "name"
  "Mobily"
  "location": {   
  "x":     
  "y": 
      }  
 "distance"  
 "isWithin20M" 
 "ports_total" 
 "ports_used"
 }
 ------
 Failure Response:
     {  "code": 
        "message": 
     } 
     
 5.{base url}/5g/{yx}
  Request :Input the lon and lat value separated by comma 
  Successful Response:
   {
  "id":
"strength":
"polygon":[
   {
    "x":
    "y":
   },
   {
    "x":
    "y":
    } 
  ]
  } 
 Failure Response:
     {  "code": 
        "message": 
     } 
  
