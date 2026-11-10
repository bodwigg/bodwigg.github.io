---
layout: page
title: Photography — Ulf Bodin
---

[Home](index.md) · [Projects](projects.md) · [Photography](photography.md)

# Photography

I’m in love with dark, high-contrast, colourful, clean, and sharp images. I often use image stitching to achieve wider angles or square compositions. I post-process my images to recreate the mood and feeling of the moment. I never add elements to my pictures, though I sometimes merge multiple captures into one. Occasionally I use AI-assisted features in Adobe Lightroom Classic to create masks and make selective edits.

## Portfolio

A selection of some of my [favourite photographs](portfolio.md).

## Photo archive

<div class="photo-card" style="float: right; width: auto; margin: 0 0 1em 1.5em; text-align: center">
  <a id="latest-photo" href="/flickr-last/"><img id="latest-photo-img" alt="My latest photo on Flickr" style="width: 200px; max-width: 100%"></a>
  <div class="caption" id="latest-photo-caption" style="max-width: 200px">My latest photo on Flickr</div>
</div>
<script>
  /* The latest photo on Flickr – from the archive's data, updated every night (see /flickr-last/). */
  fetch('/flickr-archive/data/last.json', { cache: 'no-cache' })
    .then(function (r) { if (!r.ok) throw new Error(r.status); return r.json(); })
    .then(function (p) {
      var img = document.getElementById('latest-photo-img');
      /* A thumbnail: at most 200 px on the long side. 320 px (_n) or, on sharp screens, 800 px (_c). */
      var c = p.medium.replace(/_b\.jpg$/, '_c.jpg');
      var ratio = p.ratio || 1.5;
      var w = Math.round(ratio >= 1 ? 200 : 200 * ratio);
      img.srcset = p.small + ' 320w, ' + c + ' 800w';
      img.sizes = w + 'px';
      img.src = p.small;
      img.style.width = w + 'px';
      img.style.height = 'auto';
      img.alt = p.title || 'My latest photo on Flickr';
      var caption = document.getElementById('latest-photo-caption');
      caption.textContent = p.title || 'Untitled';
      caption.appendChild(document.createElement('br'));
      caption.appendChild(document.createTextNode('Latest on Flickr'));
    })
    .catch(function () { document.getElementById('latest-photo-img').hidden = true; });
</script>

All my public Flickr photos – more than 6 700 – in [one interactive archive](/flickr-archive/). Updated from Flickr every night.

## Map

View more than 6 000 of my georeferenced photos on a [map](/flickr-archive/?geo=1) in the archive.

## Flickr

I’ve been using Flickr since 2007 and love the platform.

* [My Flickr Page](https://www.flickr.com/photos/ulfbodin/)
* [My Flickr Data Lifeboat Showcase](https://datalifeboat.flickr.org/showcase) with some images captured around my home: [Uppsala at Home – A Neighbourhood Archive](https://datalifeboat.flickr.org/dl-showcase/Ulf_Bodin-Upsala/README.html)
* A [Flickr blog post](https://blog.flickr.net/en/2025/12/16/building-flickr-archives-with-data-lifeboat/) about the Data Lifeboat

If you are interested to use my images in commercial work or hire me for a photo shoot, please contact me by Flickr mail or [email](/#contact)

## Gear

I currently use a [Canon EOS R5](/flickr-archive/?camera=Canon+EOS+R5) and a selection of Canon RF lenses – see them all under [Gear in the archive](/flickr-archive/#gear). Body swapping history:

* 1978 - 2000: Olympus OM 1 -> Olympus OM 2n -> Leica M6 ->
* 2000 - 2009: Olympus C-2040 Zoom -> [Sigma Dp 1](/flickr-archive/?camera=SIGMA+DP1) -> [Canon EOS 500D](/flickr-archive/?camera=Canon+EOS+500D) ->
* 2009 - 2018: [Canon EOS 5D II](/flickr-archive/?camera=Canon+EOS+5D+Mark+II) -> [Canon EOS 5D III](/flickr-archive/?camera=Canon+EOS+5D+Mark+III) -> [Canon EOS 5Ds R](/flickr-archive/?camera=Canon+EOS+5DS+R) ->
* 2018 - : [Canon EOS R](/flickr-archive/?camera=Canon+EOS+R) -> **[Canon EOS R5](/flickr-archive/?camera=Canon+EOS+R5)**
