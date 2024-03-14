# AWS Cloud Cost Optimization - Stale Resource Identification

Discovering and managing redundant resources is pivotal for optimizing AWS cloud costs. In this instance, we focus on identifying and managing stale Elastic Block Store (EBS) snapshots to mitigate unnecessary storage expenses.

## Description:

This Lambda function systematically identifies EBS snapshots no longer linked to any active EC2 instance, thereby paving the way for cost-effective storage management. By traversing all EBS snapshots within the account and retrieving a roster of active EC2 instances—both running and stopped—the function meticulously examines each snapshot's associated volume. If a snapshot lacks any ties to an active instance, signaling its obsolescence, the function promptly initiates its removal, thereby fostering efficient cost optimization practices within the AWS ecosystem.
