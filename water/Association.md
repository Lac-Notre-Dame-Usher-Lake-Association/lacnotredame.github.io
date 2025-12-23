---
layout: association
title: Join the Association
description: Information on how to join the Association
date: 2025-09-02
---
## Joignez notre association! -- Join our Association!

<div>
<img src="/assets/img/Winter-scenes-slide-show.pptx" class="img-fluid py-3"/>
</div>

<div style="margin-bottom: 15px;">
  <input id="/assets/img/Winter-scenes-slide-show.pptx" type="file" accept=".pptx" />
  <p>Select a PowerPoint presentation (.pptx) file for preview</p>
</div>
<div id="pptx-wrapper" style="width: 640px; height: 360px; margin: 0 auto;"></div>

 // import {init} from 'pptx-preview'; // NPM import
    import { init } from 'https://esm.sh/pptx-preview@1.0.5'; // CDN import
    // Initialize ppt previewer
    const pptxPreviewer = init(document.getElementById('pptx-wrapper'), {
      width: 640,
      height: 360
    });

    // Expose to global for file input usage
    window.pptxPreviewer = pptxPreviewer;

    // Initialize event listener
    document.getElementById("fileInput").addEventListener("change", handleFile, false);

    function handleFile(event) {
      const file = event.target.files[0];
      if (file) {
        const reader = new FileReader();
        reader.onload = function (e) {
          const arrayBuffer = e.target.result;
          pptxPreviewer.preview(arrayBuffer);
        };
        reader.readAsArrayBuffer(file);
      }
    }
  
## Renouvellement pour 2025 - Renew for 2025
* OPTION 1 : Envoyer 25 $ par Interac / Send $25 by e-transfer : [info@lacnotredame.org](mailto:info@lacnotredame.org)
  
* OPTION 2 :
