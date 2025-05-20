<p align="center">
  <a href="http://swe-bench.github.io">
    <img src="docs/assets/figures/banner.png" style="height: 10em" alt="swe-bench-live" />
  </a>
</p>

<p align="center">
  <em>A fork of SWE-bench that allows you to run its evaluation harness on the SWE-bench-Live dataset.</em>
</p>

---

> For more docs, refer to [SWE-bench/SWE-bench](https://github.com/SWE-bench/SWE-bench).

## 🚀 Set Up

```bash
# Python >= 3.10
pip install -e .
```

Test your installation by running:
```bash
python -m swebench.harness.run_evaluation \
    --dataset_name SWE-bench-Live/SWE-bench-Live \
    --split lite \
    --instance_ids amoffat__sh-744 \
    --namespace starryzhang \
    --predictions_path gold \
    --max_workers 1 \
    --run_id validate-gold
```
> Instance-level Docker images are hosted on [DockerHub](https://hub.docker.com/repositories/starryzhang).