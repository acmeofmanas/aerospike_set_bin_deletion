# aerospike_set_bin_deletion

truncate set can be used to delete bins when bins quota breached.
but before doing that below checklist is must:
1. bin/sets you have planned to clear must be removed from secondary index if it's used.
2. any rbac specific to that set must be removed first
3. XDR, ignore/ship sets must be removedd before deletion
4. you can do rolling restart of service
