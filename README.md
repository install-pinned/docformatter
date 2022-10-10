

# install-pinned/docformatter

![](https://shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)

Securely install the latest [docformatter](https://pypi.org/project/docformatter/) release from PyPI.

This action installs a pinned version of **docformatter** and all its dependencies,         making sure that file hashes match. Pinning your dependencies stops supply chain attacks where an adversary         replaces docformatter or one of its dependencies with malicious code.

## Usage

In your GitHub Actions workflow, use this action like so:

```yaml
- name: Install docformatter from PyPI
  uses: install-pinned/docformatter@d97a3897f8b7a4c3b096177ce89d06e87a127006  # 1.5.0
```

## Alternatives

This action is a relatively simple wrapper around the fantastic [pip-tools](https://pip-tools.rtfd.io)         and is most useful if there is no existing `requirements.txt`/`poetry.lock`/... infrastructure in place.         If you already pin all your dependencies in a single place, you don't need it!

## More Details

See the [@install-pinned README](https://github.com/install-pinned) for details.
