# Flentas-Assessment


**Repository Structure**
- `Task1/` — Networking & Subnetting (VPC, public/private subnets, IGW, NAT)
- `Task2/` — EC2 Static Website Hosting (Nginx on EC2 in public subnet)
- `Task3/` — High Availability + Auto Scaling (ALB, Target Group, Launch Template, ASG)
- `Task4/` — Billing & Free Tier Cost Monitoring (CloudWatch alarm / budgets)
- `Task5/` — Architecture Diagram (draw.io file and exported PNG/SVG)
  

**Task-specific notes**
- `Task1`: Outputs include VPC ID, public and private subnet IDs, IGW and NAT Gateway IDs. CIDR plan used (example): VPC `10.0.0.0/16`; public `10.0.1.0/24`, `10.0.2.0/24`; private `10.0.11.0/24`, `10.0.12.0/24`.
- `Task2`: The EC2 user-data script installs Nginx and places a static resume page at `/usr/share/nginx/html/index.html`. Confirm site by accessing the instance public IP on port 80.
- `Task3`: The ALB is internet-facing and forwards to targets in private subnets. Ensure health checks and target group settings are correct before scaling.
- `Task4`: Billing alarms and free-tier alerts require that Billing metrics are enabled for your account. When deploying, confirm the alarm currency and threshold (example: ₹100).
- `Task5`: The draw.io (`.drawio` or `.xml`) file and exported PNG/SVG are stored in `Task5/`.

**Screenshots to collect (per task)**
- Task1: VPC page, Subnets list, Route Tables, NAT Gateway + Internet Gateway.
- Task2: EC2 instance page, Security Group rules, Browser showing website.
- Task3: ALB configuration, Target Group, Auto Scaling Group, EC2 instances launched by ASG.
- Task4: Billing Alarm configuration page, Free Tier usage alerts page.
- Task5: Architecture diagram (PNG/SVG copy).
