# patient-registration
#%RAML 1.0
title: patient and registration1
description: To create the unique id of patient and registration

/add-information of patient:
  post:
    body:
      application/json:
        example:
         {
           ' "patients_name": "ABC"
          "patients age": "XY"
          "mail id": "abc@gmail.com"
          "medical record": "ab" 
          "medical record number": "m123"
          "patients category": " xyz" 
          "patients vist history": "xyz"
         "conuslt doctor" : "abc"'
         }
   
    responses:
      200:
       body:
         application/json:
           example:
             {
              
              "message":"registration successfull"
             }
    responses:
      400:
       body:
         application/json:
           example:
             {
              
              "message":"registration unsucessfull"
             }         
