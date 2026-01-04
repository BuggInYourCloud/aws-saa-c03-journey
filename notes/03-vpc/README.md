# Virtual Private Cloud (VPC)

## Key Concepts

### CIDR Ranges
| CIDR | IPs | AWS Usable |
|------|-----|------------|
| /16 | 65,536 | 65,531 |
| /20 | 4,096 | 4,091 |
| /24 | 256 | 251 |
| /28 | 16 | 11 |

AWS reserves 5 IPs per subnet (first 4 + last 1)

### NACLs vs Security Groups
| Feature | NACL | Security Group |
|---------|------|----------------|
| Level | Subnet | Instance/ENI |
| State | Stateless | Stateful |
| Rules | Allow + Deny | Allow only |
| Evaluation | Numbered order | All rules |
| Default | Allow all | Deny inbound |

### VPC Endpoints
| Type | Gateway | Interface |
|------|---------|-----------|
| Services | S3, DynamoDB | Everything else |
| Cost | Free | Hourly + data |
| HA | Built-in | Per-AZ ENI |

## Exam Tips

- NAT Gateway = managed, per-AZ, needs EIP
- NAT Instance = self-managed, can be bastion
- VPC Peering is non-transitive
- Transit Gateway = hub-and-spoke at scale

## My Notes

