# tym83.github.io

A bridge for addresses that moved to the [kuberoot-dev](https://github.com/kuberoot-dev) organization.

- `https://tym83.github.io/kubepkg-recipes/index.yaml` keeps serving the signed package index of [kuberoot-dev/kubepkg-recipes](https://github.com/kuberoot-dev/kubepkg-recipes), byte for byte, with its signature, until **2027-01-10**. Its publishing workflow updates this copy on every release. Point clusters at `https://kuberoot-dev.github.io/kubepkg-recipes/index.yaml` before then; the signing key is the same.
- Pages under `https://tym83.github.io/kubepkg/` redirect to [kuberoot-dev.github.io/kubepkg](https://kuberoot-dev.github.io/kubepkg/).

On 2027-01-10 the publishing workflow removes the copy of the index, so a cluster still using the old address reports that it cannot load the repository instead of silently staying on a stale index.
