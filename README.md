# API RESPONSE FOR GIS AND DMS


```http
GET /{base url}/health
```
 ### successful Response:
    
   ```javascript
     {
      "status"
      "odbCount"
      "fiveGCount"
      "postGisVersion"
    }
   ```
   

```http    
POST /{base url}/import/odb
```
   ## Request - Import the .kmz file
   ### Success Response:
   
   ```javascript
     {  "data":   
        "status": 
     }
   ```
      
     
   ### Failure Response:
    
   ```javascript
     {  "code": 
        "message": 
     }
   ```

```http    
POST /{base url}/fiveg/odb
``` 
   ## Request - Import the .kmz file
   ### Success Response:
   
   ```javascript
     {  "data":   
        "status": 
     }
   ```
   ### Failure Response:
  
   ```javascript
     {  "code": 
        "message": 
     }
   ```
```http        
GET /{base url}/odb/{yx}  
```
  ###  Request :Input the lon and lat value separated by comma along with provider and type 
  ###  Successful Response:
  
   ```javascript
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
  ```
 
 ### Failure Response:
 
   ```javascript
     {  "code": 
        "message": 
     } 
   ```  

```http        
GET /{base url}/5g/{yx}  
```
  ### Request :Input the lon and lat value separated by comma 
  ### Successful Response:
  
  ```javascript
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
 ```   
 ### Failure Response:
  
  ```javascript
     {  "code": 
        "message": 
     } 
   ```  
  
