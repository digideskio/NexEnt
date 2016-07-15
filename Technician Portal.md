##End Points
The actual naming of the routes can still be decided, but for now we can work with the following.
```
  /jobs
  /technicians
  /config/jobs/gridcolumns
```

##Sample data for each end-point
###/jobs
Array of job objects
```json
{
   "jobs":[
      {
         "primaryCustomerId":56,
         "primaryCustomerCode":"3MI0054",
         "customerId":56,
         "customerCode":"3MI0054",
         "customerName":"3M/IATD Division Engineering",
         "jobId":1071,
         "jobNumber":"0001072-1",
         "taskId":1650,
         "jobSubmittedDtm":"2016-06-21T11:20:00",
         "jobCompletedDtm":null,
         "jobScheduledDtm":"2016-06-21T17:21:00",
         "workOrderId":1089,
         "workOrderTypeId":3,
         "workOrderTypeCode":"CALLIN",
         "workOrderTypeText":"Customer Called in",
         "machineId":6,
         "machineSerialNumber":"0004361",
         "machineUnitId":"",
         "machineLocation":"",
         "machineDescription":"40,000lb x 5lb",
         "modelId":4,
         "modelClass":"Rice Lake",
         "modelNumber":"RL 480",
         "modelDescription":"",
         "jobTypeId":5,
         "jobTypeCode":"REP",
         "jobTypeText":"Repair",
         "jobPriorityId":10,
         "jobPriorityText":"Medium",
         "contractId":null,
         "contractTypeId":"",
         "contractTypeText":"",
         "jobCommentText":"test test",
         "jobIsOpen":true,
         "jobWorkPerformed":null,
         "jobPoNumber":"",
         "jobPmDue":false,
         "jobPmPerformed":false,
         "technicianId":64002,
         "technicianCode":"74500",
         "technicianName":"Chris Gutierrez",
         "technicianPhone":null,
         "technicianEmail":"xx.com",
         "technicianAssignedDtm":"2016-06-21T17:21:00",
         "requesterId":0,
         "requesterTitle":null,
         "requesterFirstName":null,
         "requesterMiddleInitial":null,
         "requesterLastName":null,
         "requesterPhone":null,
         "requesterPhoneExtension":null,
         "requesterPhoneOther":null,
         "requesterEmail":null,
         "jobStatusId":0,
         "jobStatusText":null,
         "taskStatusId":1,
         "taskStatusText":"Open",
         "taskIsOpen":true,
         "jobEttr":0.0,
         "jobIsEstimated":false,
         "resolutionCodeId":0,
         "resolutionCodeText":null
      }
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
