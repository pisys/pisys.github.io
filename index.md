---
layout: default
header: boldheader.html
---


## Supported currencies


<div class="currencies">
    {% for currency in site.data.stats.currencies %}

    {% assign curr = currency[0] %}
    {% assign stats=currency[1] %}

        {% include currency.html currency=curr stats=stats %}
    {% endfor %}
</div>

## Features

<ul class="features d-flex flex-row flex-wrap w-100">
{% for feature in site.data.features %}
    <li><i class="{{feature.collection | default: "fa" }} fa-{{ feature.icon }}"></i> <strong>{{ feature.heading }}</strong> <div>{{ feature.text }}</div></li>
{% endfor %}
</ul>

## Example

<div class="container">
  <p class="text-center m-auto"><img src="{{ "/assets/img/GraphSense_0.4.1-screenshot_detail.png" | relative_url }}" alt="screenshot"></p><p class="text-center">An example Bitcoin address, its connections and statistics.</p>
</div>

## Publications

<div class="container">
  <p>Some more technical details about GraphSense are described <a href="http://ceur-ws.org/Vol-1695/paper20.pdf">here</a>; please cite as:</p>

  <div class="highlighter-rouge"><div class="highlight"><pre class="highlight"><code>@inproceedings{Haslhofer:2016a,
    title={O Bitcoin Where Art Thou? Insight into Large-Scale Transaction Graphs.},
    author={Haslhofer, Bernhard and Karl, Roman and Filtz, Erwin},
    booktitle={SEMANTiCS (Posters, Demos)},
    year={2016}
  }
  </code></pre></div></div>

  <p>So far, GraphSense has been used for computing statistics in the following
  scientific papers:</p>

  <p>Paquet-Clouston, M., Romiti, M., Haslhofer, B., Charvat, T.
  <strong>Spams meet Cryptocurrencies: Sextortion in the Bitcoin Ecosystem</strong>
  Advances in Financial Technologies, 2019.
  <a href="https://arxiv.org/abs/1908.01051">(pdf)</a></p>

  <p>Romiti, M., Judmayer, A., Zamyatin, A., Haslhofer, B.
  <strong>A Deep Dive into Bitcoin Mining Pools: An Empirical Analysis of Mining Shares.</strong>
  Workshop on the Economics of Information Security, 2019.
  <a href="https://arxiv.org/abs/1905.05999">(pdf)</a></p>

  <p>Paquet-Clouston, M., Haslhofer, B., & Dupont, B.
  <strong>Ransomware payments in the bitcoin ecosystem.</strong>
  Journal of Cybersecurity, 5 (1).
  <a href="http://arxiv.org/abs/1804.04080">(pdf)</a></p>

  <p>Filtz, E., Polleres, A., Karl, R., Haslhofer, B.:
  <strong>Evolution of the Bitcoin Address Graph - An Exploratory Longitudinal Study.</strong>
  International Data Science Conference (DSC 2017), Salzburg, Austria, 2017.
  <a href="https://aic.ai.wu.ac.at/~polleres/publications/filtz-etal-2017IDSC.pdf">(pdf)</a></p>
</div>


## Contributors

<ul class="contributors container d-flex flex-row flex-wrap m-auto justify-content-around">
  <li><img src="{{ "/assets/img/bh.jpeg" | relative_url }}"/><a href="http://bernhardhaslhofer.info/">Bernhard Haslhofer</a></li>
  <li><img src="{{ "/assets/img/rs.png" | relative_url }}"/>Rainer Stütz</li>
  <li><img src="{{ "/assets/img/romitim.png" | relative_url }}"/><a href="https://matteoromiti.github.io/">Matteo Romiti</a></li>
  <li><img src="{{ "/assets/img/mr.jpeg" | relative_url }}"/><a href="https://pi.systems">Matthias Rella</a></li>    
  <li><img src="{{ "/assets/img/mb.jpeg" | relative_url }}"/>Mihai Bartha</li>    
</ul>
