# Simple Storage Service (S3)

## Key Concepts

### Storage Classes
| Class | Use Case | Retrieval | Min Duration |
|-------|----------|-----------|--------------|
| Standard | Frequent access | Instant | None |
| Intelligent-Tiering | Unknown patterns | Instant | None |
| Standard-IA | Infrequent | Instant | 30 days |
| One Zone-IA | Non-critical, infrequent | Instant | 30 days |
| Glacier Instant | Archive, instant | Instant | 90 days |
| Glacier Flexible | Archive | 1-12 hours | 90 days |
| Glacier Deep Archive | Long-term | 12-48 hours | 180 days |

### Encryption Options
- **SSE-S3**: S3 managed keys (default)
- **SSE-KMS**: KMS managed keys (audit trail)
- **SSE-C**: Customer provided keys
- **CSE**: Client-side encryption

### Replication
- **CRR**: Cross-Region Replication
- **SRR**: Same-Region Replication
- Requires versioning on both buckets

## Exam Tips

- S3 is strongly consistent (read-after-write)
- Object Lock = WORM (compliance/governance)
- Presigned URLs = temporary access
- Transfer Acceleration = CloudFront edge locations

## My Notes

