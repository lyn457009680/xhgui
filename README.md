mongodb：

use admin;
db.adminCommand({setParameter:1, internalQueryExecMaxBlockingSortBytes:536870912})

use xhprof;
db.results.createIndex({"meta.simple_url": -1})
