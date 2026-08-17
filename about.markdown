---
theme: jekyll-theme-primer
layout: sub-page
title: FFRM
permalink: /about/
---
<section class="bg-gray-light container-lg p-responsive py-4 py-md-6 my-lg-6 fade-in-center">
<div class="text-center fade-in-center">
  <h2 class="alt-h3 mb-4">About FFRM </h2>
  <div class="container-lg p-responsive py-4 py-md-6 ">
    <div class="col-md-12 animate-out mb-2">
      <!-- CMS:section id=about_about_ffrm -->
      <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
        <strong>FFRM</strong> utilises a Pyomo-based optimisation framework to endogenously calculate stranded cost, taking into consideration commercial and market issues. It uses projections for capacity and production of fossil fuel power plants to explore their retirement profile under two types of price regimes: PPA and Market Price regime. The model assesses at what capacity fossil fuel power plants become stranded and explores how this influences total compensation for stranded plants. 
        
        The model is designed to complement more detailed long-term capacity expansion models, such as OSeMOSYS, TIMES, LEAP, and others, but can also be used as a standalone retirement model. 
      </p>
      <!-- /CMS:section -->
    </div>
    <h2 class="aboutpage-subtitle text-left mb-3 mt-lg-6" id="more-than-just-code">What does it aim to do?</h2>
    <div class="col-md-12 animate-out mb-2">
      <!-- CMS:section id=about_what_does_it_aim_to -->
      <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
      The objective function of the model is set as maximisation of the net revenue at the fossil fuel power plants fleet, based on either: 
      
      Financial analysis of Power Purchase Agreements (PPAs), where these are in place with known contractual terms. 
      
      Economic optimization of the market price, where marginal costs derived from a least-cost planning are considered. 
      
      The difference in net revenue between the BAU and a decarbonization scenario is used as a measure of foregone revenue. 
      </p>
      <!-- /CMS:section -->
    </div>
  </div>
</div>

<!-- Icon Links -->
<div class="icon-links-section">
  <div class="icon-links-wrapper">
    <!-- GitHub Repository -->
    <div class="icon-link-item">
      <a href="https://github.com/FossilFuelRetirementModel/ffrm_python " target="_blank">
        <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="80" height="80" alt="GitHub" />
        <h3 class="aboutpage-subtitle text-primary">GitHub Repository</h3>
      </a>
    </div>

    <!-- Model Documentation -->
    <div class="icon-link-item">
      <a href="https://ffrm-python.readthedocs.io/en/latest/index.html" target="_blank">
        <img src="/assets/img/Rtdicon.png" width="80" height="80" alt="ReadTheDocs icon" />
        <h3 class="aboutpage-subtitle text-primary">Model Documentation</h3>
      </a>
    </div>
  </div>
</div>

  

<style>
.fade-in-center {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeInUp 1s ease forwards;
}
@keyframes fadeInUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.alt-h3 {
  font-size: 1.15rem;
}
@media (min-width: 768px) {
  .row.justify-content-center > .col-md-4 {
    margin-bottom: 2rem;
  }
}
</style>

