# AWS Incident Nightmares Every SRE Should Know

**Real Production Failure Patterns and How to Investigate Them**

Download the printable PDF version:\
<a href="../assets/pdf/aws_incident_nightmares_sre_guide v1.pdf" style="min-width:260px; border:1px solid #e5e7eb; border-radius:8px; padding:12px; text-decoration:none;">AWS Incident Nightmares SRE Guide</a>

------------------------------------------------------------------------

## Why This Guide Exists

Production incidents rarely appear as clean failures.

Instead engineers often encounter:

-   ambiguous signals
-   cascading retries
-   misleading metrics
-   partial system behaviour

Recognising failure **patterns early** dramatically reduces incident
resolution time.

This guide summarises **10 failure patterns that repeatedly appear in
AWS-based systems**.

------------------------------------------------------------------------

## 10 AWS Incident Nightmares

### 1. API Gateway 502 / 504 Storms

**Symptoms** - sudden spike of gateway errors - multiple downstream
services affected

**Typical Cause** - backend integration timeout

**First Investigation** Check backend service latency and integration
logs.

------------------------------------------------------------------------

### 2. Lambda Cold Start Failures

**Symptoms** - first requests after deployment slow or failing

**Typical Cause** - dependency loading delays

**First Investigation** Review Lambda init duration and startup logs.

------------------------------------------------------------------------

### 3. DynamoDB Throttling Cascades

**Symptoms** - retries increasing exponentially - latency spikes

**Typical Cause** - exceeded provisioned capacity

------------------------------------------------------------------------

### 4. Retry Amplification Loops

**Symptoms** - traffic spike during outage

**Typical Cause** - retry logic without exponential backoff

------------------------------------------------------------------------

### 5. Partial Deployments

**Symptoms** - some instances behave differently

**Typical Cause** - incomplete rollout

------------------------------------------------------------------------

### 6. Dependency API Outages

Internal services fail due to upstream API outages.

------------------------------------------------------------------------

### 7. Configuration Drift

Environment behaves differently without new deployment.

------------------------------------------------------------------------

### 8. Silent Data Corruption

Incorrect results without errors.

------------------------------------------------------------------------

### 9. Resource Exhaustion

Containers restart due to CPU or memory pressure.

------------------------------------------------------------------------

### 10. Queue Backlogs

System appears healthy but processing slows.

------------------------------------------------------------------------

## How Engineers Use These Patterns

During incidents:

1.  Identify failure shape
2.  Confirm pattern in logs
3.  Run targeted CloudWatch searches

------------------------------------------------------------------------

## Related Investigation Resources

Start with the **2AM Incident Investigation Cheat Sheet**.

Then apply structured log searches from:

**AWS Log Search Recipes**
