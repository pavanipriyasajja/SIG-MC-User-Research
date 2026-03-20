## User Research - Choosing the right method

The SIG Multi-Cluster team is working to build solutions for engineers operating multi-cluster environments, understanding those engineers’ needs and experiences was a critical first step.

Since the SIG Multi Cluster is still in the early stage of solution development. So we followed user research method selection guidelines, that explains if we wanted to learn about the product which is still in the early stage the Surveys are the best and effective methods to capture feedback from a broad audience (engineers) responsible for deploying, monitoring, and managing multi-cluster setups. We decided to do multi cluster surveys. 

## Survey guidelines

After finalizing the user research methods, we developed the survey guidelines to ensure the survey was clear, accessible, and able to reach a broader audience within the guidelines. 

Along with that, making sure that the survey reaches the right participants.
Here is the documents that explain the survey design guidelines for our multi-cluster project: <a href="https://docs.google.com/document/d/1exnFgQBCGLHqu9dcIxv4rr9eggKSezOmpvIG-T0clyE/edit?usp=sharing">Document</a> 

## What were we included in our survey?
Once we created the guidelines, now it’s time to understand and list our target audience, problem statement, goals, focusing on the questionnaires preparations, Time line, Survey creating format and distribution platforms, Expected number of participants. 
Learn more from this proposal document:  <a href="https://docs.google.com/document/d/1uCyHpI5zV1ME9qBtGjLkrIhpl3iXe-zQsn0SSbBiAE4/edit?usp=sharing">Document</a> 

<b>Our target audience</b>

Engineers who are responsible for multi cluster operations - Deploying, monitoring, debugging and maintenance.

<b>Survey questionnaires preparations</b>

In our survey we included a <b>total 21</b> number of questions = <b>Quantitative 13 + Qualitative 8</b>, With two sections such as participant information and cluster setup overview.

While developing the survey questions, we ensured they covered multi-cluster-related problems and engineers’ expectations, with a focus on workflows, tooling, operational challenges, use cases, and architecture. 
We shared our questionnaire during the multi-cluster team meeting and received feedback from multiple engineers. The questions were finalized after five rounds of revisions and iterations with the SIG teammates. 

Here is the list of qualitative and quantitative finalized questions.

<b>The quantitative questions:</b>

<ol>
<li>Name</li> 
<li>Why does your organization have, and run, multiple clusters?  What's the primary benefit for your use-cases?</li>
  
<li>What challenges have you encountered when diagnosing issues that span multiple clusters?</li>

<li>How do you usually respond to a critical alert affecting multiple clusters?</li>

<li>What are the most common bottlenecks you encounter when managing multicluster workloads?</li>

<li>If you could improve one aspect of your multicluster monitoring setup, what would it be?</li>

<li>Are there any use cases, tools, or challenges we didn’t cover that you think are important to highlight?</li>

<li>If you're also interested in participating in a follow-up user research interview, you can optionally provide your email at the end of the survey.</li>
</ol>

<b>The The quantitative questions includes</b> 

<ol style="line-height: 2;">
  <li style="margin-bottom: 24px;">
    What is your primary role in managing Kubernetes clusters?
    <ul>
      <li>DevOps Engineer</li>
      <li>Platform Engineer</li>
      <li>Site Reliability Engineer</li>
      <li>Cloud Engineer</li>
      <li>Software Developer</li>
      <li>Other: _______</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    How many clusters do you manage, or deploy to, currently (Per month)?
    <ul>
      <li>1-3</li>
      <li>4-10</li>
      <li>11-50</li>
      <li>50+</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    Where are your clusters deployed? (Select all that apply)
    <ul>
      <li>Single Cloud Provider (e.g., AWS, Azure, GCP)</li>
      <li>Multi-Cloud (clusters across multiple cloud providers)</li>
      <li>On-premise data centers</li>
      <li>Hybrid (mix of cloud and on-prem)</li>
      <li>Edge locations</li>
      <li>Other: _______</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    What is the typical tenancy model of your clusters?
    <ul>
      <li>Mostly Single-Tenant (one team/project per cluster)</li>
      <li>Mostly Multi-Tenant (multiple teams share clusters)</li>
      <li>A mix of both</li>
      <li>Not sure / Prefer not to say</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    Which of the following best describes how application teams interact with clusters in your organization? (Choose the option that most closely matches your setup)
    <ul>
      <li>A. Application teams manage their own clusters, have full control, and use any Kubernetes resources they need</li>
      <li>B. A platform team owns the clusters, gives app teams a namespace (single or multi-cluster), and app teams deploy via Git repositories using allowlisted resources</li>
      <li>C. A centralized infra team manages the clusters, app teams get a folder in a Git repo, and deploy using CRDs provided by the platform team</li>
      <li>D. Clusters are managed by a dedicated cluster team, app teams receive Git access, and use open-source CRDs they choose themselves</li>
      <li>E. Other (please describe): __________________</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    Which of the tools below do you, or other people on your team, use frequently and rely on for multi-cluster operations? (Select all that apply)
    <ul>
      <li>Custom controllers</li>
      <li>Rancher</li>
      <li>GKE Fleet (or Anthos)</li>
      <li>Amazon EKS Anywhere</li>
      <li>Azure Arc</li>
      <li>OpenShift Advanced Cluster Management (ACM)</li>
      <li>Open Cluster Management</li>
      <li>Karmada</li>
      <li>Kubefed</li>
      <li>Admiralty</li>
      <li>KubeAdmiral</li>
      <li>Istio (Multi-Primary / Multi-Cluster)</li>
      <li>Submariner</li>
      <li>Cilium ClusterMesh</li>
      <li>Argo CD (with multi-cluster setup)</li>
      <li>Flux CD</li>
      <li>Thanos (for multi-cluster observability)</li>
      <li>Kyverno (for cross-cluster policy enforcement)</li>
      <li>OPA Gatekeeper</li>
      <li>Other (please specify): ___________</li>
      <li>I don't use any multi-cluster tools</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    What challenges have you experienced when using multi-cluster tools? (Select all that apply)
    <ul>
      <li>Complexity in setup and configuration</li>
      <li>Lack of clear documentation</li>
      <li>Integration issues with cloud/on-prem environments</li>
      <li>Policy enforcement across clusters</li>
      <li>Multi-tenancy isolation or access control</li>
      <li>Observability and debugging across clusters</li>
      <li>Networking and service discovery between clusters</li>
      <li>Scalability concerns</li>
      <li>Limited support or community activity</li>
      <li>Other (please specify): ___________</li>
      <li>No major challenges</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    What metrics do you track most frequently across clusters? (Select top 3)
    <ul>
      <li>CPU and memory utilization</li>
      <li>Pod health and readiness</li>
      <li>Network latency between clusters</li>
      <li>Service availability</li>
      <li>Persistent volume usage</li>
      <li>Policy compliance</li>
      <li>Other: ______</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    How do you identify the root cause of a workload issue when it spans multiple clusters?
    <ul>
      <li>Logs</li>
      <li>Metrics</li>
      <li>Alerts</li>
      <li>Network tracing</li>
      <li>Manual investigation</li>
      <li>Automated diagnostic tools</li>
      <li>Other: _______</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    What kind of alerts do you find most useful in a multi-cluster setup?
    <ul>
      <li>Cluster health degradation</li>
      <li>Pod crashes or restarts</li>
      <li>Inter-cluster network issues</li>
      <li>API server unresponsiveness</li>
      <li>Inconsistent workload placement</li>
      <li>Other: _______</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    What would you want from a centralized observability dashboard for multiple clusters? (Select all that apply)
    <ul>
      <li>A unified view of workload health</li>
      <li>Cross-cluster log aggregation</li>
      <li>Real-time alerts and incident tracking</li>
      <li>Policy compliance and security monitoring</li>
      <li>Visual cluster topology map</li>
      <li>Automated issue detection or root cause analysis</li>
      <li>Ability to customize queries and dashboards</li>
      <li>Prebuilt dashboards with minor adjustments</li>
      <li>Out-of-the-box dashboards (no customization needed)</li>
      <li>I don't need a centralized observability dashboard</li>
      <li>Other (please specify): ___________</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    Which types of automated responses would you like to see for handling cross-cluster issues? (Select all that apply)
    <ul>
      <li>Automated failover</li>
      <li>Auto-scaling based on workload health</li>
      <li>Policy-based workload redistribution</li>
      <li>Alert escalation without action</li>
      <li>No automation - manual intervention preferred</li>
    </ul>
  </li>

  <li style="margin-bottom: 24px;">
    In your opinion, what role should a "ClusterProfile" play in managing and operating multiple Kubernetes clusters? (Select all that apply)
    <ul>
      <li>Keeping an inventory of clusters with metadata (e.g., name, region, owner)</li>
      <li>Defining and enforcing standard configurations across clusters</li>
      <li>Grouping clusters by environment, region, or purpose</li>
      <li>Acting as a source of truth for GitOps workflows</li>
      <li>Linking clusters with platform policies, add-ons, or compliance rules</li>
      <li>Tracking lifecycle events (creation, updates, deletion)</li>
      <li>I'm not sure</li>
      <li>I don't see a role for ClusterProfile</li>
    </ul>
  </li>
</ol>


<b>Survey distribution method and format</b>

We decided to use Google Forms to collect survey responses, along with another accessible format in a GitHub file so that everyone could easily access the list of questionnaires even after the survey had ended. 
Here is the survey link: <a href="https://forms.gle/34d7WB3odepjxFEt7">link</a> 

We distributed our surveys through SIG-Multicluster, <b>Kubernetes.io</b> (Name= "end user facing") and <b>k8sContributors</b>(Name="contributor/developer facing") socials (X, Mastodon, BlueSky, LinkedIn)"

<b>Expected number of participants >100.</b>

<b>Time line</b>

Our survey remained open for participants to submit responses over an <b>8-week period</b>, giving most people enough time to participate.

<b>Resources</b>

Here is a list of resources we used while creating the survey.

Detailed information of conducting surveys: <a href="https://youtu.be/_ToDcKzeXBc?si=W8zBNEEWZVt5j0-L">link</a> 

Why most of the engineers interested in conducting the surveys: <a href="https://dev.to/priya_sajja_c336921bbda87/why-do-the-majority-of-the-engineering-teams-focus-on-conducting-the-surveys-2h72">link</a> 
