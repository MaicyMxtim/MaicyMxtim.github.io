---
layout: default
---

<header class="hero">
<p class="kicker">Maicy Maritim · Platform Engineering</p>
<h1>Building cloud platforms that are secure, observable and easy to operate.</h1>
<p class="sub">I am a data science graduate who moved into infrastructure because I enjoyed building the systems behind software more than the models themselves. I work on Kubernetes, cloud infrastructure, automation and developer tooling.</p>
<ul class="chips">
<li>AWS</li><li>Kubernetes</li><li>Terraform</li><li>GitOps</li><li>Python</li>
</ul>
<div class="cta">
<a class="btn primary" href="#featured">View projects</a>
<a class="btn ghost" href="https://github.com/MaicyMxtim">GitHub</a>
</div>
<div class="stats">
<div class="stat reveal"><span class="n">95&nbsp;ms</span><span class="l">p95 latency in production, against a 400&nbsp;ms target</span></div>
<div class="stat reveal"><span class="n">100%</span><span class="l">of deployments delivered through GitOps</span></div>
<div class="stat reveal"><span class="n">57%</span><span class="l">projected AI spend saving from measured model tiering</span></div>
<div class="stat reveal"><span class="n">449/450</span><span class="l">requests answered while five failures were caused on purpose</span></div>
</div>
</header>

<h2 id="featured">Featured project</h2>

<article class="project reveal">
<p class="role">Live on AWS</p>
<h3><a href="https://maicymxtim.github.io/tamani-platform/">Tamani Platform</a></h3>
<p>An internal developer platform running a real venue discovery backend on Kubernetes in AWS, deployed and reachable on the public internet.</p>
<ul class="stack">
<li>AWS</li><li>OpenTofu</li><li>k3s</li><li>Argo CD</li><li>Kyverno</li><li>NATS</li><li>Prometheus</li><li>Anthropic API</li>
</ul>
<p class="question">Built to answer one question: how do you let developers ship AI-backed services safely without needing infrastructure expertise?</p>

<div class="diagram">
<svg viewBox="0 0 780 470" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Tamani Platform architecture diagram">
<defs>
<marker id="arr1" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
<path d="M 0 0 L 10 5 L 0 10 z" class="dg-arr"/>
</marker>
</defs>

<rect x="20" y="44" width="160" height="36" rx="8" class="dg-box"/>
<text x="100" y="66" text-anchor="middle" class="dg-t">GitHub · main</text>
<line x1="100" y1="80" x2="100" y2="102" class="dg-line" marker-end="url(#arr1)"/>

<rect x="20" y="104" width="160" height="52" rx="8" class="dg-box"/>
<text x="100" y="126" text-anchor="middle" class="dg-t">GitHub Actions</text>
<text x="100" y="143" text-anchor="middle" class="dg-s">test · scan · SBOM · sign</text>
<line x1="100" y1="156" x2="100" y2="178" class="dg-line" marker-end="url(#arr1)"/>

<rect x="20" y="180" width="160" height="36" rx="8" class="dg-boxa"/>
<text x="100" y="202" text-anchor="middle" class="dg-a">Argo CD</text>
<line x1="180" y1="198" x2="218" y2="198" class="dg-line" marker-end="url(#arr1)"/>

<rect x="249" y="20" width="140" height="32" rx="8" class="dg-box"/>
<text x="319" y="40" text-anchor="middle" class="dg-t">Internet</text>
<line x1="319" y1="52" x2="319" y2="98" class="dg-line" marker-end="url(#arr1)"/>

<rect x="220" y="86" width="540" height="316" rx="12" class="dg-zone"/>
<text x="740" y="110" text-anchor="end" class="dg-s">k3s on AWS · state reconciled from Git</text>

<rect x="244" y="100" width="150" height="36" rx="8" class="dg-box"/>
<text x="319" y="122" text-anchor="middle" class="dg-t">ingress · TLS</text>
<line x1="319" y1="136" x2="319" y2="168" class="dg-line" marker-end="url(#arr1)"/>

<rect x="244" y="170" width="150" height="48" rx="8" class="dg-box"/>
<text x="319" y="190" text-anchor="middle" class="dg-t">venue API</text>
<text x="319" y="206" text-anchor="middle" class="dg-s">FastAPI</text>

<rect x="414" y="170" width="170" height="48" rx="8" class="dg-boxa"/>
<text x="499" y="190" text-anchor="middle" class="dg-a">AI gateway</text>
<text x="499" y="206" text-anchor="middle" class="dg-s">budgets · cache · ledger</text>

<rect x="604" y="170" width="140" height="48" rx="8" class="dg-box"/>
<text x="674" y="190" text-anchor="middle" class="dg-t">agents</text>
<text x="674" y="206" text-anchor="middle" class="dg-s">governed runtime</text>
<line x1="604" y1="194" x2="586" y2="194" class="dg-line" marker-end="url(#arr1)"/>

<line x1="319" y1="218" x2="319" y2="244" class="dg-line" marker-end="url(#arr1)"/>
<line x1="499" y1="218" x2="509" y2="244" class="dg-line" marker-end="url(#arr1)"/>

<rect x="244" y="246" width="170" height="48" rx="8" class="dg-box"/>
<text x="329" y="266" text-anchor="middle" class="dg-t">NATS JetStream</text>
<text x="329" y="282" text-anchor="middle" class="dg-s">events · retries · DLQ</text>

<rect x="444" y="246" width="140" height="48" rx="8" class="dg-box"/>
<text x="514" y="266" text-anchor="middle" class="dg-t">Redis</text>
<text x="514" y="282" text-anchor="middle" class="dg-s">queue · cache</text>

<rect x="244" y="330" width="250" height="44" rx="8" class="dg-box"/>
<text x="369" y="349" text-anchor="middle" class="dg-t">Prometheus · Grafana · Loki</text>
<text x="369" y="365" text-anchor="middle" class="dg-s">SLOs · burn-rate alerts</text>

<rect x="514" y="330" width="230" height="44" rx="8" class="dg-boxa"/>
<text x="629" y="349" text-anchor="middle" class="dg-a">Kyverno admission</text>
<text x="629" y="365" text-anchor="middle" class="dg-s">signed images only</text>

<rect x="220" y="418" width="540" height="34" rx="8" class="dg-box"/>
<text x="490" y="439" text-anchor="middle" class="dg-s">AWS · EC2 · Route 53 · S3 · SSM Parameter Store · IAM</text>
</svg>
</div>

<ul class="badges">
<li>100% GitOps delivery</li>
<li>Signed images with SBOMs</li>
<li>Kyverno admission control</li>
<li>Governed AI gateway</li>
<li>Per-tenant cost budgets</li>
<li>SLOs with burn-rate alerts</li>
<li>Governed autonomous agents</li>
<li>Service scaffold to live in 195&nbsp;s</li>
</ul>
<p class="links">
<a href="https://maicymxtim.github.io/tamani-platform/">Read the case study →</a>
<a href="https://platform.waypear.com/">Live site</a>
<a href="https://github.com/MaicyMxtim/tamani-platform">Code</a>
</p>
</article>

<h2>Also built</h2>

<article class="project reveal">
<p class="role">MLOps</p>
<h3><a href="https://maicymxtim.github.io/akili/">Akili Platform</a></h3>
<p>An MLOps platform that retrains a model, decides whether the new version should replace the live one, deploys it gradually and rolls back on its own. Its reliability was tested by causing real failures while traffic was running.</p>
<ul class="stack">
<li>k3d</li><li>Argo CD</li><li>Argo Workflows</li><li>MLflow</li><li>Feast</li><li>Argo Rollouts</li><li>Evidently</li><li>Kyverno</li>
</ul>
<p class="question">Built to answer one question: how much of the machine learning lifecycle can run safely without a person involved?</p>

<div class="diagram">
<svg viewBox="0 0 810 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Akili Platform pipeline diagram">
<defs>
<marker id="arr2" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
<path d="M 0 0 L 10 5 L 0 10 z" class="dg-arr"/>
</marker>
</defs>

<rect x="20" y="40" width="112" height="48" rx="8" class="dg-box"/>
<text x="76" y="60" text-anchor="middle" class="dg-t">new data</text>
<text x="76" y="76" text-anchor="middle" class="dg-s">780k sales</text>
<line x1="132" y1="64" x2="150" y2="64" class="dg-line" marker-end="url(#arr2)"/>

<rect x="152" y="40" width="112" height="48" rx="8" class="dg-box"/>
<text x="208" y="60" text-anchor="middle" class="dg-t">validate</text>
<text x="208" y="76" text-anchor="middle" class="dg-s">reject bad files</text>
<line x1="264" y1="64" x2="282" y2="64" class="dg-line" marker-end="url(#arr2)"/>

<rect x="284" y="40" width="112" height="48" rx="8" class="dg-box"/>
<text x="340" y="60" text-anchor="middle" class="dg-t">train</text>
<text x="340" y="76" text-anchor="middle" class="dg-s">MLflow tracked</text>
<line x1="396" y1="64" x2="414" y2="64" class="dg-line" marker-end="url(#arr2)"/>

<rect x="416" y="40" width="112" height="48" rx="8" class="dg-boxa"/>
<text x="472" y="60" text-anchor="middle" class="dg-a">promotion gate</text>
<text x="472" y="76" text-anchor="middle" class="dg-s">better, or refused</text>
<line x1="528" y1="64" x2="546" y2="64" class="dg-line" marker-end="url(#arr2)"/>

<rect x="548" y="40" width="112" height="48" rx="8" class="dg-box"/>
<text x="604" y="60" text-anchor="middle" class="dg-t">canary rollout</text>
<text x="604" y="76" text-anchor="middle" class="dg-s">auto-rollback</text>
<line x1="660" y1="64" x2="678" y2="64" class="dg-line" marker-end="url(#arr2)"/>

<rect x="680" y="40" width="112" height="48" rx="8" class="dg-box"/>
<text x="736" y="60" text-anchor="middle" class="dg-t">serving API</text>
<text x="736" y="76" text-anchor="middle" class="dg-s">signed model</text>

<rect x="20" y="130" width="772" height="38" rx="8" class="dg-box"/>
<text x="406" y="153" text-anchor="middle" class="dg-s">3-node k3d cluster · Argo CD · Argo Workflows · Prometheus · Grafana · Loki · Evidently drift checks</text>
</svg>
</div>

<ul class="badges">
<li>Automated promotion gate</li>
<li>Canary rollouts with auto-rollback</li>
<li>Signed models and images</li>
<li>Monthly drift detection</li>
<li>Point-in-time correct features</li>
<li>Chaos-tested reliability</li>
</ul>
<p class="links">
<a href="https://maicymxtim.github.io/akili/">Read the case study →</a>
<a href="https://github.com/MaicyMxtim/akili">Code</a>
</p>
</article>

<h2>Engineering philosophy</h2>

<div class="reveal">
<p>Each of my projects starts from a practical engineering question and builds a working answer to it.</p>
<ul class="questions">
<li>How can deployment be made safer and more repeatable?</li>
<li>How can a platform give developers self-service without losing control?</li>
<li>How can AI workloads be kept inside a budget?</li>
<li>How do you show, with evidence, that a system is reliable?</li>
</ul>
</div>

<h2>Background</h2>

<div class="reveal">
<p>I studied data science and started out on the modelling side. While working on those projects I found that I enjoyed the infrastructure more than the models, so I changed direction. Since then I have built and operated two platforms end to end, from infrastructure as code and cluster setup through to monitoring, incident reports and cost analysis.</p>
<ul class="timeline">
<li>Data science</li>
<li class="arrow">→</li>
<li>ML systems</li>
<li class="arrow">→</li>
<li>Platform engineering</li>
<li class="arrow">→</li>
<li class="now">Open to roles</li>
</ul>
</div>

<h2>Skills</h2>

<div class="skills">
<div class="skill-group reveal"><h4>Cloud</h4><p>AWS: EC2, Route 53, S3, SSM, IAM</p></div>
<div class="skill-group reveal"><h4>Orchestration</h4><p>Kubernetes (k3s, k3d), Docker</p></div>
<div class="skill-group reveal"><h4>Infrastructure as code</h4><p>Terraform, OpenTofu</p></div>
<div class="skill-group reveal"><h4>Delivery</h4><p>GitHub Actions, Argo CD, Argo Workflows, Argo Rollouts</p></div>
<div class="skill-group reveal"><h4>Security &amp; supply chain</h4><p>Kyverno, cosign, trivy, syft, gitleaks, External Secrets Operator</p></div>
<div class="skill-group reveal"><h4>Observability</h4><p>Prometheus, Grafana, Loki, Evidently</p></div>
<div class="skill-group reveal"><h4>Services &amp; languages</h4><p>Python, FastAPI, NATS, Redis, Bash, Linux</p></div>
<div class="skill-group reveal"><h4>ML platform</h4><p>MLflow, Feast, DVC, LightGBM</p></div>
</div>

<footer>
<p class="status">Currently looking for platform engineering, DevOps, site reliability, cloud engineering and infrastructure roles.</p>
<nav>
<a href="mailto:maicymaritim@gmail.com">Email</a>
<a href="https://github.com/MaicyMxtim">GitHub</a>
<a href="https://www.linkedin.com/in/maicy-maritim/">LinkedIn</a>
</nav>
</footer>
