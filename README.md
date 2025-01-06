### ModernBERT sample project

The repository contains a sample project for using the ModernBERT model. It's using [`uv` for dependency managment](https://docs.astral.sh/uv/), and notebooks for running the code.

Make sure to restore the dependencies before running the notebooks:
```bash
uv sync
```

After that you can open the notebooks in your favorite Jupyter environment (which clearly should be VSCode) and start experimenting with the ModernBERT model!

The `ModernBert.ipynb` notebook contains the two samples for using two versions of the model:
* base model used on fill-mask task ([`answerdotai/ModernBERT-base`](https://huggingface.co/answerdotai/ModernBERT-base))
* [PyLate](https://github.com/lightonai/pylate) model used for multi-vector retrieval task ([`joe32140/ColModernBERT-base-msmarco-en-bge`](https://huggingface.co/joe32140/ColModernBERT-base-msmarco-en-bge))

> [!NOTE]
> The repository is using [forked version of PyLate](https://github.com/Krzysztof-Cieslak/pylate/pull/1) - the only changes I've done was bumping dependencies to the pre-release version of `transformers` (required for `ModernBERT`)