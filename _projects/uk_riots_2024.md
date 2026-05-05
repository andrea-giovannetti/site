---
layout: page
title: The 2024 Riots of Merseyside
description: Tracing the path from online activity to offline mobilisation
img: assets/img/projects/riots_network_full.png
importance: 2
category: policy
related_publications: "vergani2026ukriots"

---

_On 29 July 2024 a knife attack at a Taylor Swift-themed dance class in [Southport, Merseyside](https://en.wikipedia.org/wiki/2024_Southport_stabbing) killed three children. Within hours, online discourse seeded a wave of riots that spread across England. With [Matteo Vergani](https://experts.deakin.edu.au/27631-Matteo-Vergani) (Deakin) and the [Tackling Hate Lab](https://tacklinghate.org/), this work asks a deceptively simple question: <strong>can online hate and political discourse signal, or even anticipate, real-world violence?</strong> The answer, we argue, is not in raw post volumes but in the architecture of the networks that carry the content._

**[[Full Report (Tackling Hate Lab)]](https://tacklinghate.org/wp-content/uploads/2026/04/The-2024-UK-Riots_LowRes.pdf)** &nbsp; **[[Lab Insights]](https://tacklinghate.org/lab-insights/the-2024-uk-riots-tracing-the-path-from-online-activity-to-offline-mobilisation/)**

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The 2024 Riots of Merseyside</title>
</head>
<body>
    <div class="post">
        <article>
            <div class="row">
                <div class="col-md-6">
                    <section>
                        <h2>Context</h2>
                        <p>The 2024 UK riots were the most serious episode of public disorder in England in over a decade, with confirmed offline incidents in 37 locations and a sequence of attacks on hotels housing asylum seekers. Existing research on digital mobilisation typically describes online hate descriptively, but offers little empirical evidence on the link between online discourse and offline collective violence. Policy stakeholders - from <a href="https://www.homeaffairs.gov.au/">Home Affairs</a> in Australia to <a href="https://www.merseyside.police.uk/">Merseyside Police</a> in the UK - need an evidence base that goes beyond word counts.</p>
                    </section>
                    <section>
                        <h2>Aims</h2>
                        <p>We test whether online dynamics can <em>signal</em> or <em>anticipate</em> real-world violence, and we identify the structural features of the online network that carry that signal. The work situates the UK riots within debates on misinformation, hate speech, and networked mobilisation, and compares the UK case against an Australian discourse baseline collected over the same window.</p>
                    </section>
                    <section>
                        <h2>Methodology</h2>
                        <p>We assemble three geolocated datasets: <strong>67,934</strong> UK tweets, <strong>5,388</strong> Australian comparison tweets, and <strong>85</strong> verified offline incidents across 37 UK locations. We construct a directed reaction network of <strong>47,341 nodes</strong> (including 326 far-right accounts) and <strong>189,030 edges</strong> (1,698 between far-right accounts). Anti-foreigner and anti-politics narratives are scored through LLM-based classifiers; community structure is recovered with clustering algorithms; and online–offline alignment is tested with Hawkes-process models. The methodology is fully reproducible.</p>
                    </section>
                </div>

                <div class="col-md-6">
                    <div class="figure-container text-center mb-4">
                        {% include figure.html path="assets/img/projects/riots_network_full.png" title="The pro/anti-riot reaction network" class="img-fluid rounded z-depth-1" %}
                        <div class="caption" style="text-align: left;">
                            <strong>Figure 1.</strong> Full directed reaction network on X during the 2024 UK riots. Green edges encode anti-riot content, red edges pro-riot content; node size is proportional to influence. The pro-riot component sits in a dense red core at the bottom of the graph, while anti-riot content is concentrated in a single green spine. Pro-riot views are diffused across multiple clusters; anti-riot views are tightly concentrated within one.
                        </div>
                    </div>
                    <div class="figure-container text-center mb-4">
                        {% include figure.html path="assets/img/projects/riots_clusters.png" title="Cross-cluster influence and the hard-core component" class="img-fluid rounded z-depth-1" %}
                        <div class="caption" style="text-align: left;">
                            <strong>Figure 2.</strong> A small set of high-influence accounts (orange/blue clusters, top-left) project red (pro-riot) reactions over a vast, fragmented audience (right). The figure visualises a defining feature of the riots: a tightly-connected pocket of <em>hard-core</em> pro-riot users captures the lion's share of the network's flows.
                        </div>
                    </div>
                    <div class="figure-container text-center">
                        {% include figure.html path="assets/img/projects/riots_amplifiers.png" title="Influencers vs amplifiers" class="img-fluid rounded z-depth-1" %}
                        <div class="caption" style="text-align: left;">
                            <strong>Figure 3.</strong> Influencers (top-of-graph nodes) generate the content; amplifiers (bottom-of-graph mass) spread it. The two roles are structurally distinct, and the <em>reposting rate</em> - not the volume of original content - is the empirical signal that aligns most tightly with offline unrest.
                        </div>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-md-12">
                    <section>
                        <h2>Key Findings</h2>
                        <ul>
                            <li><strong>Spikes in online hate align with offline unrest, but raw volume does not predict violence.</strong> The signal lives in the network architecture, not in the post counts.</li>
                            <li><strong>Extreme concentration of influence.</strong> The top 100 users drive <strong>54% of all network reactions</strong>; the top 10 alone drive <strong>15%</strong>. These accounts have enormous traction with very limited reciprocal engagement.</li>
                            <li><strong>A measurable Australian footprint.</strong> Several of the most influential UK accounts have non-trivial reach in the Australian information ecosphere - a finding directly relevant to Australian CVE policy.</li>
                            <li><strong>Pro-riot users form a tightly-connected hard core</strong>, while anti-riot users are concentrated within a single cluster. Pro-riot content is therefore harder to attenuate by content moderation alone.</li>
                            <li><strong>Influencers are not amplifiers.</strong> The accounts that originate hostile narratives are structurally distinct from those that spread them. <em>The control of flows lies within a small pocket of users.</em></li>
                            <li><strong>Reposting rate is a strong early-warning signal.</strong> Original posts containing hostile narratives rise <em>before</em> riots; retweets peak <em>during</em> the violence, marking the transition from mobilisation to amplification.</li>
                        </ul>
                    </section>
                    <section>
                        <h2>Policy Implications</h2>
                        <ul>
                            <li><strong>Monitor what mobilises and spreads, not what is loudest.</strong> Reposting structures and cross-cluster amplification are operationalisable early-warning indicators that move past simple keyword volumes.</li>
                            <li><strong>Target the small bottleneck of cross-cluster amplifiers.</strong> Because the top 10 accounts capture 15% of reaction flows, even narrow, evidence-based interventions can have outsized de-escalation effects without broad-based content moderation.</li>
                            <li><strong>Treat anti-foreigner and anti-politics narratives as <em>distinct</em> mobilisation channels.</strong> They evolve at different speeds and recruit different audiences.</li>
                            <li><strong>Australian relevance.</strong> The same network primitives operate on the Australian X graph, and the UK case provides a transferable template for stress-testing Australian online ecosystems before similar events.</li>
                        </ul>
                    </section>
                    <section>
                        <h2>Future Research</h2>
                        <ul>
                            <li>Extend the Hawkes-process tests across a panel of 2024-2025 UK and Australian shock events to identify a generalisable set of early-warning signatures.</li>
                            <li>Integrate offline-incident data at finer geographic resolution (LSOA / SA2 level) to test the spatial reach of online amplification.</li>
                            <li>Develop a real-time dashboard for stakeholder partners that operationalises the reposting-rate signal as an actionable monitoring tool.</li>
                        </ul>
                    </section>
                </div>
            </div>
        </article>
    </div>

<div class="team-members">
  <h2>Team:</h2>
  <ul>
    <li><strong>A/Prof Matteo Vergani, Deakin University</strong> (<a href="mailto:matteo.vergani@deakin.edu.au">matteo.vergani@deakin.edu.au</a>)</li>
    <li><strong>Dr Andrea Giovannetti, Australian Catholic University</strong> (<a href="mailto:andrea.giovannetti@acu.edu.au">andrea.giovannetti@acu.edu.au</a>)</li>
    <li><strong>A/Prof Kewen Liao, Australian Catholic University</strong> (<a href="mailto:kewen.liao@acu.edu.au">kewen.liao@acu.edu.au</a>)</li>
    <li><strong>Dr Xinzhe Li, Australian Catholic University</strong></li>
    <li><strong>Stephanie Zi Xin Ng, Deakin University</strong> (<a href="mailto:szng@deakin.edu.au">szng@deakin.edu.au</a>)</li>
    <li><strong>Dan Goodhardt, Tackling Hate Lab</strong></li>
  </ul>
</div>

</body>
</html>
