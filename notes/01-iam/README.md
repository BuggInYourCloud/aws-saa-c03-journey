# IAM, Accounts & AWS Organizations

## Key Concepts

### IAM Policy Evaluation
```
Explicit Deny > Explicit Allow > Implicit Deny
```

### ARN Format
```
arn:aws:service:region:account:resource
```

### Policy Types
- **Identity-based**: Attached to users/groups/roles
- **Resource-based**: Attached to resources (S3, SQS, etc.)
- **Permission boundaries**: Max permissions for IAM entities
- **SCPs**: Max permissions for org accounts

## Cheatsheet

| Component | Purpose |
|-----------|---------|
| Users | Individual identities |
| Groups | Collections of users |
| Roles | Temporary credentials |
| Policies | Permission documents |
| SCPs | Org-level guardrails |

## Exam Tips

- Roles > Access keys for EC2
- Cross-account access = trust policy + permissions
- SCPs don't grant permissions, only restrict
- Root account can't be restricted by SCPs

## My Notes

*Detailed notes in Obsidian vault*

- ✅ Completed Module 1: Course Fundamentals & AWS Accounts (8/9 lessons)
- Remaining: AWS CLI v2 setup demo

