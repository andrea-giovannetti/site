---
layout: page
title: Home Affairs - Countering Violent Extremism (Phase 2)
description: Network dynamics of online hate in post-7 October Australia
img: assets/img/projects/cve_network_post7oct.png
importance: 3
category: policy
related_publications: "giovannetti2025dro"

---

_This is Phase 2 of the [National Countering Violent Extremism Research Project](https://www.homeaffairs.gov.au/about-us/our-portfolios/national-security/countering-terrorism/countering-violent-extremism), funded by the [Department of Home Affairs](https://www.homeaffairs.gov.au/). In this project, we document and decompose the surge in online antisemitic and Islamophobic hate in Australia following the Hamas attacks of 7 October 2023 - and we show that the post-7-October hate ecosystem is built around the pre-existing one._

**[[Public Report: Unveiling Influence Flows in Online Anti-Jewish and Anti-Muslim Hate in Australia (Deakin DRO)]](https://dro.deakin.edu.au/articles/report/Unveiling_Influence_Flows_in_Online_Anti-Jewish_and_Anti-Muslim_Hate_in_Australia/31975407)**

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Affairs - Countering Violent Extremism (Phase 2)</title>
</head>
<body>
    <div class="post">
        <article>
            <div class="row">
                <div class="col-md-6">
                    <section>
                        <h2>Context</h2>
                        <p>Following the Hamas attacks on Israel on 7 October 2023 and the subsequent war, Australia recorded a sustained surge in reported online Islamophobic and antisemitic incidents. Public reporting documents the surge but is silent on the <em>complex processes operating in the background</em>: who drives the hate, how the audience changes, and whether the post-7-October ecosystem is a continuation of the pre-existing one or a fundamentally new phenomenon. This project answers those questions with a unique, multi-year dataset.</p>
                    </section>
                    <section>
                        <h2>Aims</h2>
                        <p>We deliver to the Department of Home Affairs an empirical, network-level account of the structure and evolution of online antisemitic and Islamophobic hate in the Australian X/Twitter ecosphere; we identify the small subset of users who carry most of the hate flows; and we test whether the post-7-October surge is built around incumbent users or driven by newcomers.</p>
                    </section>
                    <section>
                        <h2>Methodology</h2>
                        <p>We assemble a unique panel of <strong>1,926,376 actions</strong> (posts, shares, replies) by <strong>100,542 Australian-based users</strong>, covering October 2022 through March 2025. Collection follows a curated lexicon of more than 200 keywords and combinations capturing antisemitic and Islamophobic discourse. Each message is scored for <em>toxicity</em> via the Google Perspective API. We treat the resulting graph as a directed influence network where an edge from user <em>i</em> to user <em>j</em> records that <em>j</em> reacted to a post by <em>i</em>. Community detection groups users that share narratives, and pre/post-7-October comparisons isolate the change in network structure attributable to the shock.</p>
                    </section>
                </div>

                <div class="col-md-6">
                    <div class="figure-container text-center mb-4">
                        {% include figure.html path="assets/img/projects/cve_toxicity_surge.png" title="The post-7-October surge" class="img-fluid rounded z-depth-1" %}
                        <div class="caption" style="text-align: left;">
                            <strong>Figure 1.</strong> Top: monthly unique users producing antisemitic and Islamophobic content on the Australian X graph; the dashed red line marks 7 October 2023. Bottom: total monthly toxicity (blue) and toxicity per action (red), showing that hateful content not only became <em>more frequent</em> but also <em>more toxic per message</em>, and stayed there. By March 2025 an average of ~4,000 messages per month carry antisemitic or Islamophobic content.
                        </div>
                    </div>
                    <div class="figure-container text-center mb-4">
                        {% include figure.html path="assets/img/projects/cve_network_pre7oct.png" title="Influence network: Pre-7 October" class="img-fluid rounded z-depth-1" %}
                        <div class="caption" style="text-align: left;">
                            <strong>Figure 2.</strong> Influence network of antisemitic and Islamophobic hate on the Australian X graph, October 2022 to October 2023. <strong>3,922 active users</strong> (8% of the eventual base), <strong>1,401 influencers</strong>, <strong>10,910 links</strong> (just 2.33% of the eventual edges). Mean toxicity 0.92; the top 1% of users have toxicity above 0.6.
                        </div>
                    </div>
                    <div class="figure-container text-center">
                        {% include figure.html path="assets/img/projects/cve_network_post7oct.png" title="Influence network: Post-7 October" class="img-fluid rounded z-depth-1" %}
                        <div class="caption" style="text-align: left;">
                            <strong>Figure 3.</strong> Same network, October 2023 to April 2025. <strong>21,303 active users</strong> (43%), <strong>7,401 influencers</strong>, <strong>455,923 links</strong> (97.31% of the eventual edges). Mean toxicity 7.8 - and crucially, <strong>incumbent users score 6.6 times higher in toxicity than newcomers</strong>. The post-7-October graph is not a new ecosystem: 72% of the pre-7-October incumbent nodes remain interconnected, and the new mass of users grows <em>around</em> them.
                        </div>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-md-12">
                    <section>
                        <h2>Key Findings</h2>
                        <ul>
                            <li><strong>The surge is real, sustained, and qualitatively different.</strong> The number of users producing hate quintuples and toxicity per message jumps and stays elevated for at least 18 months after the shock.</li>
                            <li><strong>Incumbents - not newcomers - drive the toxicity.</strong> Users active before 7 October 2023 score on average <strong>6.6× higher in toxicity</strong> than users who entered the ecosystem after the shock.</li>
                            <li><strong>The post-shock network expands around the pre-shock cores.</strong> 72% of the pre-7-October incumbent nodes remain linked together as the network grows; the surge is structurally a <em>scaling-up</em> of an existing ecosystem, not a new one.</li>
                            <li><strong>Influence concentrates in a small group of accounts.</strong> The number of influencers rises from 1,401 to 7,401, but their share of links rises from 2.33% to 97.31% of the eventual graph - a textbook example of preferential attachment at work in a hate ecosystem.</li>
                            <li><strong>Centrality and toxicity are persistent.</strong> Users who were toxic and central before the shock remain toxic and central after, with strong substitution between toxicity and popularity at the very top of the distribution.</li>
                        </ul>
                    </section>
                    <section>
                        <h2>Policy Implications</h2>
                        <ul>
                            <li><strong>Monitor the incumbent core, not the newcomer surge.</strong> The empirical leverage of post-shock interventions is concentrated on a small, identifiable set of pre-existing users.</li>
                            <li><strong>Differentiate surge dynamics from baseline.</strong> Annual reporting indicators that count incidents miss the structural shift; network-level monitoring is the operationalisable alternative.</li>
                            <li><strong>Use toxicity-weighted, not volume-weighted indicators.</strong> Since toxicity per action and not just total volume changes after the shock, action-level scoring is necessary for accurate situational awareness.</li>
                            <li><strong>Cross-platform transferability.</strong> The methodology generalises to Telegram, Bluesky and other emerging platforms where Home Affairs and AVERT have growing monitoring needs.</li>
                        </ul>
                    </section>
                    <section>
                        <h2>Deliverables</h2>
                        <ul>
                            <li><a href="https://dro.deakin.edu.au/articles/report/Unveiling_Influence_Flows_in_Online_Anti-Jewish_and_Anti-Muslim_Hate_in_Australia/31975407">Public report</a> hosted on Deakin Research Online: <em>Unveiling Influence Flows in Online Anti-Jewish and Anti-Muslim Hate in Australia</em>.</li>
                            <li>AVERT International Research Symposium 2025 presentation (Australian Catholic University and Deakin University).</li>
                            <li>Forthcoming peer-reviewed manuscripts on (i) the incumbent-vs-newcomer toxicity gap and (ii) the persistence of centrality and toxicity in hate networks.</li>
                            <li>Stakeholder briefings for the Department of Home Affairs.</li>
                        </ul>
                    </section>
                </div>
            </div>
        </article>
    </div>

<div class="team-members">
  <h2>Team:</h2>
  <ul>
    <li><strong>Dr Andrea Giovannetti, Australian Catholic University</strong> (lead) (<a href="mailto:andrea.giovannetti@acu.edu.au">andrea.giovannetti@acu.edu.au</a>)</li>
    <li><strong>A/Prof Matteo Vergani, Deakin University</strong> (<a href="mailto:matteo.vergani@deakin.edu.au">matteo.vergani@deakin.edu.au</a>)</li>
    <li><strong>Stephanie Zi Xin Ng, Deakin University</strong> (<a href="mailto:szng@deakin.edu.au">szng@deakin.edu.au</a>)</li>
  </ul>
</div>

<div class="partners-container" style="margin-top: 2rem; display: flex; gap: 1.5rem; align-items: center; flex-wrap: wrap;">
  <a href="https://www.homeaffairs.gov.au/"><img src="{{ '/assets/img/home_affairs_logo.png' | relative_url }}" alt="Department of Home Affairs" style="max-height: 70px;"></a>
  <a href="https://tacklinghate.org/"><img src="{{ '/assets/img/taklinghate.png' | relative_url }}" alt="Tackling Hate Lab" style="max-height: 70px;"></a>
  <a href="https://www.acu.edu.au/"><img src="{{ '/assets/img/acu_logo.png' | relative_url }}" alt="Australian Catholic University" style="max-height: 70px;"></a>
  <a href="https://deakin.edu.au"><img src="{{ '/assets/img/deakin.png' | relative_url }}" alt="Deakin University" style="max-height: 70px;"></a>
</div>
 

</body>
</html>
