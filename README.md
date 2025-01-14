# RunsOn: 10x cheaper GitHub Action runners.

On-demand, self-hosted runners, for your GitHub Action workflows.

Any size, at the cheapest price available.

Runs in your own AWS account. 

Quick overview:
* Each workflow job triggers a fresh new runner (i.e. ephemeral).
* Access to all Linux runner types available on AWS.
* Supports both x64 and arm64.
* 1-1 workflow compatibility with your existing workflows.
* No concurrency limit: you can launch as many workflows in parallel as needed.
* SSH access into the runners if needed.
* 🆕 in v1.6.1: local S3 cache for greater speed with `runs-on/cache` action, and UNLIMITED cache sizes.


```diff
- runs-on: ubuntu-latest
+ runs-on: runs-on,runner=16cpu-linux,image=ubuntu22-full-x64
```
<img width="675" alt="RunsOn is the fastest and cheapest GitHub Action self-hosted runner alternative" src="https://github.com/runs-on/runs-on/assets/6114/92933f39-c173-4afd-ae43-cc7532f82f77">

## Prices

At least 2x cheaper than SaaS offerings, up to 10x cheaper than GitHub hosted runners. And the [largest choice of configs](https://instances.vantage.sh) ever. All in infrastructure that you control.

The crazy thing is that even if you use larger instance types (e.g. 16cpu) for your workflows, it might actually be cheaper than using a 2cpu instance since your workflow _should_ finish much more quickly (assuming you can take advantage of the higher core number).

→ Use the [GitHub Action pricing calculator](https://runs-on.com/calculator/) to get an idea of the savings.

## Documentation

→ [Read the RunsOn docs](https://runs-on.com/docs) for all the details.

## License

The source code for this software is open, but licensed under the [Prosperity Public License 3.0.0](https://prosperitylicense.com). In practice this means that:

* It is indefinitely free to use for non-commercial usage.

* If you install for use in a for-profit organization, you are free to install and evaluate it for 31 days, after which you must buy a license.

→ [Learn more about licensing](https://runs-on.com/pricing).

## Author

This software is built by [Cyril Rohr](https://cyrilrohr.com) - [Twitter/X](https://twitter.com/crohr).

If you like DevOps tooling, you might also be interested in my other projects [PullPreview.com](https://pullpreview.com) and [Packager.io](https://packager.io).
