# 2AM AWS Incident Investigation Cheat Sheet

Download the printable PDF version:\
`aws_log_search_2am_incident_cheat_sheet.pdf`
<a href="../assets/pdf/aws_log_search_2am_incident_cheat_sheet.pdf" style="min-width:260px; border:1px solid #e5e7eb; border-radius:8px; padding:12px; text-decoration:none;">AWS Log Search 2am Incident Cheat Sheet</a>


------------------------------------------------------------------------

## The 2AM Problem

PagerDuty fires.

CloudWatch logs explode across multiple services.

Thousands of log lines appear.

The biggest challenge is not fixing the problem ---\
it is deciding **where to start investigating**.

------------------------------------------------------------------------

## First Ask Three Questions

1.  Is the failure global or tenant-specific?
2.  Is the failure getting worse or stabilising?
3.  Did anything change recently?

------------------------------------------------------------------------

## 5‑Minute Investigation Flow

### Step 1 --- Detect Error Spike

Confirm whether errors truly increased.

### Step 2 --- Find the First Error

Identify the earliest failure event.

### Step 3 --- Check Dependency Failures

Determine whether an external service is failing.

### Step 4 --- Identify Noisiest Tenant

Determine if issue is global or isolated.

### Step 5 --- Trace Request Path

Reconstruct the lifecycle of a request.

------------------------------------------------------------------------

## Key Insight

Most incidents are **not solved by reading logs line‑by‑line**.

They are solved by running **focused pattern searches**.

------------------------------------------------------------------------

## Recommended Next Step

Use structured CloudWatch queries from:

**AWS Log Search Recipes**
