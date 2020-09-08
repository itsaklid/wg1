# WG1Template

For basf2 users:
setup your basf2 enviroment, then run

`pip install git+https://github.com/MarkusPrim/WG1Template.git`

to install the package.

## Configuration

### Enable/disable errorbar caps and top-right ticks

The recommendations of the [Belle2Style](https://stash.desy.de/projects/B2D/repos/belle2style) are not to have
top/right axis ticks or errorbar caps, but some users might still prefer them. They can be enabled by

```python
from wg1template plot_style
plot_style.set_matplotlibrc_params(errorbar_caps=True, top_right_ticks=True)
```
