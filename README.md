# WG1Template

For basf2 users:
setup your basf2 enviroment, then run

`pip install git+https://github.com/MarkusPrim/WG1Template.git`

to install the package.



## Configuration

### Align axis labels on the axes ends

To get axis labels at the axes ends, as was the default in previous versions of the WG1 template, you just
have to change some global variables that the WG1 template uses:

```python
wg1template.plot_style.xlabel_pos = {"x": 1, "ha": "right"}
wg1template.plot_style.ylabel_pos = {"x": 1, "ha": "right"}
```

### Enable/disable errorbar caps and top-right ticks

The recommendations of the [Belle2Style](https://stash.desy.de/projects/B2D/repos/belle2style) are not to have
top/right axis ticks or errorbar caps, but some users might still prefer them. They can be enabled by

```python
from wg1template plot_style
plot_style.set_matplotlibrc_params(errorbar_caps=True, top_right_ticks=True)
```
