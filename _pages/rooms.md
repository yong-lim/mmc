---
layout: rooms
title: Check Rooms Availability
---

<div class="grid">

  {%- for room in site.data.rooms -%}

  <article role="article" class="card">
    <div class="meta">
      <h2>
        <a target="_blank" rel="noopener noreferrer" href="{{ room.link }}">
          {{ room.name }}
        </a>
      </h2>
      <p>{{ room.details }}
      <br>Location:  {{ room.location }}
      <br>Capacity:  {{ room.capacity }}</p>
    </div>

  </article>

  {%- endfor -%}

</div>
