---
description: How to Contribute Back to the Avalanche Community
---

# Contribute to Avalanche

The last step to become a **real continual learning super-hero** ⚡ is to fall into a _radioactive dump_.☢️ Just kidding, it's much easier than that: you need to contribute back to _Avalanche_!

There are no _superheroes_ that are not altruistic!

{% hint style="info" %}
In order to contribute to _Avalanche_, first of all you need to become familiar with all its features and the codebase structure, so if you have not followed the _"From Zero to Hero Tutorial"_ from the beginning we suggest to do it before starting to make changes.
{% endhint %}

First of all, [install _Avalanche_ in "_Developer Mode"_](../getting-started/how-to-install.md#developer-mode-install) _if you haven't already._ After you've familiarized with the _Avalanche_ codebase you have two roads ahead of you:

1. You can start working on a [open issue](../questions-and-issues/add-your-issue.md) \(we have dozen of them!\)
2. You can [submit a feature-request](../questions-and-issues/request-a-feature.md) and propose yourself to work on it.

![Examples of Avalanche Issues available on GitHub](../.gitbook/assets/issues.png)

**In any of the two cases you'd need to follow the steps below**:

1. [Join our Slack](https://join.slack.com/t/continualai/shared_invite/enQtNjQxNDYwMzkxNzk0LTBhYjg2MjM0YTM2OWRkNDYzOGE0ZTIzNDQ0ZGMzNDE3ZGUxNTZmNmM1YzJiYzgwMTkyZDQxYTlkMTI3NzZkNjU) and **\#avalanche-dev** channel \(optional but recommended\)
2. ⭐_Star_ + 👁️wa_tch_ the repository.
3. Fork the repository.
4. Create or assign an existing issue/feature to yourself.
5. Make your changes.
6. Make a [Pull Request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-requests) \(PR\).

**The following rules should be respected:**

* Use PEP8 coding style and work within the 80 columns limit.
* Always pull before pushing a commit.
* Try to assign to yourself one issue at a time.
* Try closing an issue **within roughly 7 days**. If you are not able to do that, please break it down into multiple ones you can tackle more easily, or you can always remove your assignment to the issue!
* If you add a new feature, please include also a _test_ and a usage example in your PR.

Also, before making your PR **make sure** that the following commands return without any errors:

```bash
pycodestyle avalanche
python -m unittest discover -v
```

Otherwise fix them and run again these commands until everything is working correctly. You should also check if everything is working on GPUs, using the env variable `USE_GPU=False`:

```bash
USE_GPU=False python -m unittest discover -v
```

Faster integrity checks can be run with the env variable `FAST_TEST=True` :

```bash
USE_GPU=False FAST_TEST=True python -m unittest discover -v
```

## 🤝 Run it on Google Colab

You can run _this chapter_ and play with it on Google Colaboratory: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ContinualAI/colab/blob/master/notebooks/avalanche/6.-contribute-to-avalanche.ipynb)

