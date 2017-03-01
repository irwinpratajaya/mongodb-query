# mongodb-query

### 1. membuat database mongodb
#### input:
use academic

#### output:
switched to db academic


### 2. insert database into collection department
#### input:
db.department.insert( [
  { code: '001', name: 'economics', major: 'finance' },
  { code: '002', name: 'economics', major: 'accounting' },
  { code: '003', name: 'economics', major: 'marketing' },
  { code: '004', name: 'IT', major: 'IT' },
  { code: '005', name: 'IT', major: 'SI' }
  ]
)
#### output:
BulkWriteResult({
	"writeErrors" : [ ],
	"writeConcernErrors" : [ ],
	"nInserted" : 5,
	"nUpserted" : 0,
	"nMatched" : 0,
	"nModified" : 0,
	"nRemoved" : 0,
	"upserted" : [ ]
})

#### input:
db.student.insert( [
  {studentId: '0001', name: 'Irwin Pratajaya', address: 'Jakarta', department: 001},
  {studentId: '0002', name: 'Endy Susanto', address: 'BSD', department: 003},
  {studentId: '0003', name: 'Wahyu', address: 'Depok', department: 004}
  ]
)

#### output:
BulkWriteResult({
	"writeErrors" : [ ],
	"writeConcernErrors" : [ ],
	"nInserted" : 3,
	"nUpserted" : 0,
	"nMatched" : 0,
	"nModified" : 0,
	"nRemoved" : 0,
	"upserted" : [ ]
})


### 3. show collections
#### input:
show collections

#### output:
department
student
