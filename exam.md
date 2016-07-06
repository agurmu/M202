# FINAL EXAM

# Question 1: Config Servers 
TODO
# Question 2: Replica Set
TODO
# Question 3: Fixing a Bad Shard Key
TODO
# Question 4: Failed replica set initiation
TODO
# Question 5: Diagnosing an Event with Mtools
TODO
# Question 6: Automatic chunk splitting
TODO
# Question 7: Traffic Imbalance in a Sharded Environment

mongos>use admin

mongos>sh.status()

mongos>sh.stopBalancer()

mongos>db.runCommand( { moveChunk : "m202.imbalance", bounds : [{"_id": ISODate("2014-07-15T00:00:00Z")},{"_id": ISODate("2014-07-16T00:00:00Z")}],"to":"shard0001"})

mongos>db.runCommand( { moveChunk : "m202.imbalance", bounds : [{"_id": ISODate("2014-07-16T00:00:00Z")},{"_id": ISODate("2014-07-17T00:00:00Z")}],"to":"shard0001"})

mongos>db.runCommand( { moveChunk : "m202.imbalance", bounds : [{"_id": ISODate("2014-07-18T00:00:00Z")},{"_id": ISODate("2014-07-19T00:00:00Z")}],"to":"shard0001"})

# Question 8: Sorting in a Sharded Environment
TODO
