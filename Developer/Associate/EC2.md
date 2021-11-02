## EC2

Elastic Compute Cloud -> AWS Virtual Machine

- Complete control of your instances

- Pay for what you use (PAYG)

- Avoid wasted capacity, select capacity as you need

---

### Pricing Options

- On Demand (default)
  - Pay by the hour or second depending on the instance type
- Reserved Capacity
  - Reserved for 1 or 3 years, commit for a period of time, in return you get up to a 72% discount. These instances are region specific.
- Dedicated Instances
  - Physical server that only you can use, can be useful for strict compliance or licensing
- Spot Instances
  - Purchase unused capacity, up to 90% cheaper, availability is not guaranteed. Good for non-critical work.

---

- Reserved: predictable use, specific capacity requirements, pay upfront, cheaper

- standard reserved instances: cannot change mind (up to 75% cheaper)

- convertible reserved instances: can change to a different reserved instance type of equal or greater value (up to 54% cheaper)

- scheduled reserved instances: launch within a schedule, when capacity is predictable for fluctuations

---

- Dedicated hosts can be on-demand or reserved instances at a discount (up to 70% discount)

---

### Savings plans

- Up to 72% savings

- Commit to one or three years of capacity usage regardless of instance type or size

- Also covers serverless technology like Lambda and Fargate

---

### AWS Pricing Calculator

- Helps understand the various pricing options in AWS

---

### Instance Types

- This is the hardware used by the underlying physical server

- Capabilities, each storage type offers different cpu, memory, and storage, and are grouped into instance families

- List is growing over time

- Instance types are optimised to fit specific use cases

  - Micro instances
  - General purpose (t2)
  - Compute optimised (c5d, c5n)
  - FPGA instances (f1)
  - GPU instances (g2, g3s, g4dn, p3)
  - Machine Learning ASIC instances (inf1)
  - Memory optimised (r5ad, x1e, z1d, m2)
  - Storage optimised (d2, i2, h1)

- Numbers in the type name represent the generation for example t2 is second generation and t3 is third generation.

- Micro instances are free tier eligible

---

### SSH on Mac

- Download key

- chmod 400 somekeypair.pem

- ssh ec2-user@10.0.0.1 -i somekeypair.pem

---

### Useful Links

- https://calculator.aws/#/
