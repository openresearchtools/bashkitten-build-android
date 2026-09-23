# BashKitten android builder

Build-only repository for [BashKitten](https://github.com/openresearchtools/bashkitten).
The workflow checks out the exact product commit requested by the main workflow.
This repository owns its own compiler cache and never publishes releases.

Download the installable candidate from a run's **Actions → Artifacts** as soon
as its upload finishes. Linux candidates contain the complete browser and Agent
package; Android candidates contain the signed APK. Main collects each finished
target independently. Browser components are retained for reuse when unchanged.

Workflow source: `.github/builders/android.yml` in the product repository.
