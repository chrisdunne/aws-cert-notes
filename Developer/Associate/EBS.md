## EBS

Elastic Block Store

- Storage volumes you can attach to EC2 instances (disks, hard drives, etc)

- Use the same way you would with any system disks: - run OS - run database - use as a filesystem

- Designed for mission critical production workflows

- Highly available, with auto replication in a single AZ

- Highly Scalable, dynamically increase capacity and change volume type with zero downtime

---

### Types

### `GP2` - General Purpose SSD (solid state drive)

- 3 IOPS per GiB unto max of 16k IOPS per volume

- GP2 volumes under 1 TB in size can burst to up to 3k IOPS

- Good for boot volumes and development and test applications, which are not latency sensitive

### `io1` - Provisioned IOPS

- High performance, and most expensive EBS volume

- Up to 64k IOPS per volume, 50 IOPS per GiB.

- Use if need more than the 16k IOPS provided by GP2

- I/0 intensive applications, low latency

### `io2` - Latest generation Provisioned IOPS

- Higher durability and more IOPS per GiB, 500 IOPS per GiB

- Same price as io1 (just use io2)

- 5 9’s of durability

- High I/o intensive workloads with higher durability

### `st1` - Throughput optimised HDD

- Low cost HDD volume

- Great for storing large amounts of data, which is accessed frequently

- 40MB/s per TB throughput, burst to up to 200MB/s, with a max of 500MB/s per volume

- Frequently accessed throughput intensive workloads (Big data, data warehouse, ETL, logging)

- Cannot be a boot volume

### `sc1` - Cold HDD

- Cheapest option volume

- 12MB/s per TB, burst unto 80MB/s per TB, max throughput of 250MB/s per volume

- A good choice for cold data, infrequently accessed, lowest cost and performance is not a factor.

- Cannot be a boot volume

---

### IOPS

- Input and output operations per second

- Important metric for applications performing quick transactions, for example read/writes to a database, each can be a transaction

---

### Throughput

- The number of bits read or written per second

- Important for complex queries, large amounts of data such as reports, and the ability to deal with large data sets

---

### Tips

- EBS are highly available and scalable storage volumes you can attach to EC2 instances

- There are 5 different types available, gp2, io1, io2, st1, and sc1 (3 SSD options and 2 HDD options)

---

### Useful links

- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html
