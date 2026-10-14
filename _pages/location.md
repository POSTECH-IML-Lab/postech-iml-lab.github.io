---
layout: page
title: location
permalink: /location/
nav: true
nav_order: 9
map_id: 1E8SKAJD00Rq0Y9un6s9SniqBEXI5cBk
---

<style>
  .iml-address-map {
    overflow: hidden;
    border: 1px solid rgba(127, 127, 127, 0.2);
    border-radius: 16px;
  }
  .iml-address-map iframe {
    display: block;
    width: 100%;
    height: 520px;
    border: 0;
  }
  .iml-address-locations {
    margin-top: 2rem;
    border-top: 1px solid rgba(127, 127, 127, 0.2);
  }
  .iml-address-location {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 2rem;
    padding: 2rem 0;
    border-bottom: 1px solid rgba(127, 127, 127, 0.2);
  }
  .iml-address-location h3 {
    margin: 0 0 0.25rem;
    font-size: 1.15rem;
    font-weight: 600;
  }
  .iml-address-location p {
    margin: 0;
  }
  /* Pin colors mirror the marker colors set in the embedded Google My Map
     (lab = #E65100, PI's office = #0288D1). Update both if the map changes. */
  .iml-address-pin {
    display: inline-block;
    width: 0.8em;
    height: 0.8em;
    margin-right: 0.45em;
    border-radius: 50% 50% 50% 0;
    transform: rotate(-45deg);
  }
  .iml-address-pin--lab {
    background: #e65100;
  }
  .iml-address-pin--office {
    background: #0288d1;
  }
  .iml-address-room {
    display: block;
    margin-top: 0.15rem;
    font-size: 0.9rem;
    opacity: 0.7;
  }
  @media (max-width: 600px) {
    .iml-address-map iframe {
      height: 400px;
    }
    .iml-address-location {
      grid-template-columns: 1fr;
      gap: 0.5rem;
    }
  }
</style>

<div class="iml-address-map">
  <iframe
    title="Google Map of POSTECH PIAI (인공지능연구원) and RIST Building 4"
    src="https://www.google.com/maps/d/embed?mid={{ page.map_id }}"
    width="100%"
    height="520"
    loading="lazy"
    allowfullscreen
    referrerpolicy="no-referrer-when-downgrade"
  ></iframe>
</div>

<div class="iml-address-locations">
  <section class="iml-address-location">
    <h3><span class="iml-address-pin iml-address-pin--lab" aria-hidden="true"></span>Lab</h3>
    <p>POSTECH PIAI (인공지능연구원) <span class="iml-address-room">Room 421</span></p>
  </section>
  <section class="iml-address-location">
    <h3><span class="iml-address-pin iml-address-pin--office" aria-hidden="true"></span>Principal Investigator's Office</h3>
    <p>RIST Building 4 (RIST 4동) <span class="iml-address-room">Room 4410</span></p>
  </section>
</div>
