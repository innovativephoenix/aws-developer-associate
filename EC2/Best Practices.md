## This list of practices will help you get the maximum benefit from Amazon EC2.

# Security

1. Manage access to AWS resources and APIs using identity federation, IAM users, and IAM roles. Establish credential management policies and procedures for creating, distributing, rotating, and revoking AWS access credentials. For more information, see IAM Best Practices in the IAM User Guide.

1. Implement the least permissive rules for your security group. For more information, see Security group rules.

1. Regularly patch, update, and secure the operating system and applications on your instance. For more information about updating Amazon Linux 2 or the Amazon Linux AMI, see Manage software on your Linux instance in the Amazon EC2 User Guide for Linux Instances.

# Storage

1. Understand the implications of the root device type for data persistence, backup, and recovery. For more information, see Storage for the root device.

1. Use separate Amazon EBS volumes for the operating system versus your data. Ensure that the volume with your data persists after instance termination. For more information, see Preserve Amazon EBS volumes on instance termination.

1. Use the instance store available for your instance to store temporary data. Remember that the data stored in instance store is deleted when you stop, hibernate, or terminate your instance. If you use instance store for database storage, ensure that you have a cluster with a replication factor that ensures fault tolerance.

1. Encrypt EBS volumes and snapshots. For more information, see Amazon EBS encryption.

# Resource management

1. Use instance metadata and custom resource tags to track and identify your AWS resources. For more information, see Instance metadata and user data and Tag your Amazon EC2 resources.

1. View your current limits for Amazon EC2. Plan to request any limit increases in advance of the time that you'll need them. For more information, see Amazon EC2 service quotas.

# Backup and recovery

1. Regularly back up your EBS volumes using Amazon EBS snapshots, and create an Amazon Machine Image (AMI) from your instance to save the configuration as a template for launching future instances.

1. Deploy critical components of your application across multiple Availability Zones, and replicate your data appropriately.

1. Design your applications to handle dynamic IP addressing when your instance restarts. For more information, see Amazon EC2 instance IP addressing.

1. Monitor and respond to events. For more information, see Monitor Amazon EC2.

1. Ensure that you are prepared to handle failover. For a basic solution, you can manually attach a network interface or Elastic IP address to a replacement instance. For more information, see Elastic network interfaces. For an automated solution, you can use Amazon EC2 Auto Scaling. For more information, see the Amazon EC2 Auto Scaling User Guide.

1. Regularly test the process of recovering your instances and Amazon EBS volumes if they fail.

# Networking

- Set the time-to-live (TTL) value for your applications to 255, for IPv4 and IPv6. If you use a smaller value, there is a risk that the TTL will expire while application traffic is in transit, causing reachability issues for your instances.
