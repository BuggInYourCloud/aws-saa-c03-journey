# Elastic Compute Cloud (EC2)

## Key Concepts

### Instance Types
| Prefix | Type | Use Case |
|--------|------|----------|
| T | General | Burstable, web servers |
| M | General | Balanced workloads |
| C | Compute | CPU intensive |
| R | Memory | In-memory caching |
| X | Memory | Large-scale in-memory |
| I | Storage | High IOPS |
| D | Storage | Dense storage |
| P/G | Accelerated | GPU, ML |

### EBS Volume Types
| Type | Use Case | Max IOPS |
|------|----------|----------|
| gp3 | General SSD | 16,000 |
| gp2 | General SSD (burst) | 16,000 |
| io2 Block Express | Critical DB | 256,000 |
| io2/io1 | High perf DB | 64,000 |
| st1 | Throughput HDD | 500 |
| sc1 | Cold HDD | 250 |

### Purchase Options
| Type | Discount | Commitment | Interruptible |
|------|----------|------------|---------------|
| On-Demand | 0% | None | No |
| Reserved (1yr) | ~40% | 1 year | No |
| Reserved (3yr) | ~60% | 3 years | No |
| Spot | Up to 90% | None | Yes |
| Savings Plans | ~40-60% | $/hour | No |

### Placement Groups
| Type | Use Case | Notes |
|------|----------|-------|
| Cluster | Low latency | Single AZ, high risk |
| Spread | Critical instances | Max 7 per AZ |
| Partition | Big data | Isolated racks |

## Exam Tips

- Instance store = ephemeral, highest IOPS
- EBS = persistent, can detach/attach
- Instance metadata: http://169.254.169.254/latest/meta-data/

## My Notes

