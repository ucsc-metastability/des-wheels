# How to use with uv

Add the following to your `pyproject.toml`,

```toml
[tool.uv.sources]
des = { index = "des-github" }

[[tool.uv.index]]
name = "des-github" # or another name
url = "https://github.com/ucsc-metastability/des-wheels/releases/expanded_assets/index"
explicit = true
```

Then add the package to the dependencies list:

```diff
 dependencies = [
     ...,
+    "des>=x.x.x", # newest version
 ]
```
