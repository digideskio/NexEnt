##End Points (Routes)
The actual naming of the routes can still be decided, but for now we can work with the following.
```
  /jobs
  /technicians
  /config/jobs/gridcolumns
  /config/assets/images
```

##Format of data for each end-point
###/jobs
Array of job objects
```json
{
  "jobs":[
    {
      "RequestId": 158870,
      "TaskId": 254403,
      "TaskNumber": "0158757-1",
      "TaskCreatedDateTime": "2016-06-13T11:03:00",
      "TaskCompletedDateTime": null,
      "TaskTypeId": 3,
      "TaskTypeCode": "JAM",
      "TaskTypeDescription": "Jamming",
      "TaskPriorityId": 3,
      "TaskPriorityDescription": "Medium",
      "TaskScheduledDateTime": "2016-06-13T15:03:00",
      "TaskDescription": "need page counts for all non reported printers in Tampa. Put on board 6/13/2016",
      "TaskIsOpen": true,
      "TaskPoNumber": null,
      "TaskPmDue": false,
      "TaskIsPmPerformed": false,
      "TaskStatusId": 3,
      "TaskStatusCode": "Open",
      "TaskTechStatusId": 1,
      "TaskTechStatusCode": "Unassigned",
      "TaskIsEstimated": false,
      "TaskEttr": 0,
      "TaskTechId": -1,
      "TaskCommentInvoice": null,
      "TaskCommentFlagJob": null,
      "TaskCommentWorkPerformed": null,
      "TaskCommentNextJob": null,
      "TechnicianId": -1,
      "TechnicianName": null,
      "TechnicianCode": null,
      "TechnicianLogin": null,
      "EquipmentId": -1,
      "EquipmentContractId": -1,
      "BillToID": 9394,
      "BillToCode": "TIMCUS-BILLING",
      "CustomerID": 9398,
      "CustomerCode": "TIMCUS-TAMPA2",
      "CompanyName": "TIME CUSTOMER SERVICE INC",
      "CustomerAddress1": "3000 UNIVERSITY CENTER DR",
      "CustomerAddress2": null,
      "CustomerCity": "TAMPA",
      "CustomerState": "FL",
      "CustomerCountry": "USA",
      "CustomerPhoneText": null,
      "CustomerPhoneNumeric": null
    },
  ]
}
```
### /technicians
Array of technician objects
```json
{
   "technicians":[
      {
         "technicianId":64002,
         "technicianCode":"74500",
         "firstName":"Chris",
         "lastName":"Gutierrez",
         "phone":null,
         "email":null,
         "homeStoreId":4,
         "homeStoreCode":"MAIN",
         "homeStoreName":"Houston Scale Co. Inc."
      }
   ]
}
```
### /config/jobs/gridcolumns
Object mapping job field names to column captions
```
{
  "columns": {
    "FieldName" : "Column Name",
    ...
  }
}
```
For example
```json
{
  "columns": {
    "primaryCustomerId": "Primary Client ID",
    "primaryCustomerCode": "Primary Client Code",
    "customerId": "Client ID",
    "customerCode": "Client Code",
    "customerName": "Client Name"
  }
}
```

### /config/assets/images
Custom images for this deployment
