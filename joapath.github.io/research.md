---
layout: page
title: Research
description: CVE research — analysis, reproduction, and proof-of-concept development.
permalink: /research/
---

Each entry includes root cause analysis, a reproducible lab, and a working proof of concept.

<!-- 
  Uncomment and add rows as CVE repos are published.
  Naming convention: cve-YYYY-NNNNN-product

<table class="cve-table">
  <thead>
    <tr>
      <th>CVE</th>
      <th>Product</th>
      <th>Type</th>
      <th>Severity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="cve-id"><a href="https://github.com/Joapath/cve-2024-36401-geoserver">CVE-2024-36401</a></td>
      <td>GeoServer</td>
      <td>RCE (OGC filter injection)</td>
      <td><span class="severity sev-critical">Critical</span></td>
    </tr>
  </tbody>
</table>
-->

<div class="placeholder">First CVE research coming soon — starting with a critical RCE.</div>

## Repository structure

Each CVE gets its own repo following `cve-YYYY-NNNNN-product`:

```
cve-YYYY-NNNNN-product/
├── README.md        # Root cause, timeline, impact
├── poc/             # Proof of concept
├── lab/             # Docker setup to reproduce
├── analysis/        # Patch diff, flow diagrams
└── references/      # Advisories, patches
```
