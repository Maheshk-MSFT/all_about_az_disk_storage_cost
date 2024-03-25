### (1) Ultra disks 
          - fastest storage performance, which includes high throughput, high IOPS, and low latency-4 GB up to 64 TB
					- suitable for top-tier db's and SAP HANA 
					- 1,200 IOPS (300 MB/s) to 160,000 IOPS and 4000 MB/s 
					- if Premium SSD managed disks have caused performance bottlenecks, consider using Ultra disks.
					
### (2) Premium SSD v2
					- Unlike Premium SSD managed disks, Premium SSD v2 managed disks don't have dedicated sizes.
					- 1 GB-64TB
					- 3,000-80,000 (Increases by 500 IOPS per GiB)
					- 125-1,200 (increases by 0.25 MB/s per set IOPS)
					- any supported size you prefer
					- Premium SSD v2 managed disks are suited for a broad range of workloads such as SQL server, Oracle, MariaDB, SAP, Cassandra, Mongo DB, big data/analytics, and gaming, on virtual machines or stateful containers.

### (3) Premium SSD	
				- next tier down from Premium SSD v2 managed disks in terms of performance, but they still provide high throughput and IOPS with low latency
				- P4, P15, P40, P80 
				- 32 GB to 32 TB
				- 120 IOPS to 20,000 IOPS
				- 25 MB/s to 900 MB/s 
				-  Premium SSD managed disks are a good fit for mission-critical workloads in medium and large organizations.
				- this disks support two bursting models, an on-demand bursting model and a credit-based model. 

### (4) Standard SSD managed disks
				- cost-effective storage option for VMs that need consistent performance at lower speeds.
				- 	still provide single-digit millisecond (ms) latencies and up to 6,000 IOPS and 750 MB/s of throughput. 
				- E4, E15, E40, E80 
				- 32 GB - 32 tB
				- 500 IOPS to 6000 IOPS
				- 60 MB/s to 750 MB/s 
				
### (5) Standard HDD managed disks
				- data is stored on conventional magnetic disk drives that have moving spindles. Disks are slower and the variation in speeds is higher compared to solid-state drives (SSDs)
				- S4, S15, S40, S80
				- 32 GB to 32 TB
				- 500 IOPS to 2000 IOPS
				- 60 MB/s to 500 MB/s 
				- minimize costs for less critical workloads and development or test environments.
			
** Performance plus (preview) ** 
The Input/Output Operations Per Second (IOPS) and throughput limits for Premium SSD, Standard SSD, and Standard HDD that are 513 GiB and larger can be increased by enabling performance plus. 
https://learn.microsoft.com/en-us/azure/virtual-machines/disks-enable-performance?tabs=azure-cli
- Enabling performance plus (preview) improves the experience for workloads that require high IOPS and throughput, such as database and transactional workloads. There's no extra charge for enabling performance plus on a disk.
-- Can only be enabled on new disk
--Not supported for disks recovered with Azure Site Recovery or Azure Backup.
-- Can't be enabled in the Azure portal.
-- https://learn.microsoft.com/en-us/training/modules/optimize-performance-and-costs-using-azure-disk-storage/
