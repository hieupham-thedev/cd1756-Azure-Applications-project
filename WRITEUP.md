# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

## Student Input
*Cost Analysis: With same memory and compute power, we choose **App Service** which have lower costs*
<table>
<tr>
<th>Virtual Machine</th>
<th>App Service</th>
</tr>
<tr>
<td>
VM Size: DS1_v2<br>
Family: General purpose<br>
vCPUs: 1<br>
RAM (GiB): 3.5<br>
Data disks: 4<br>
Max IOPS: 3200<br>
Temp storage (GiB): 7<br>
Premium disk: Supported<br>
Cost/month: $41.61<br>
</td>
<td>
Pricing tiers: B2<br>
<br>
200 total ACU<br>
RAM (GiB): 3.5<br>
A-Series compute equivalent<br>
<br>
<br>
<br>
Cost/month: $25.55<br>
</td>
</tr>
</table>

*Scalability Analysis: With our simple app and undefined scaling requirement, **App Service** has built-in autoscale service and integrated load balancer which will adapt to scaling requirement when needed*
<table>
<tr>
<th>Criteria</th>
<th>Virtual Machine</th>
<th>App Service</th>
</tr>
<tr>
<td>Autoscaling</td>
<td>Virtual machine scale sets</td>
<td>Built-in service</td>
</tr>
<tr>
<td>Load Balancer</td>
<td>Azure Load Balancer</td>
<td>Integrated</td>
</tr>
</table>

*Availability Analysis: Both VM and App Service guarantee available 99.95% of the time*