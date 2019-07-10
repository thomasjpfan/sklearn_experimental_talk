# Implementing Experimental

[Link to presentation slides](https://github.com/thomasjpfan/sklearn_experimental_talk/blob/master/presentation.pdf)

```python
# sklearn/experimental/enable_hist_gradient_boosting.py
from ..ensemble._hist_gradient_boosting.gradient_boosting import (
    HistGradientBoostingClassifier,
    HistGradientBoostingRegressor
)

from .. import ensemble

ensemble.HistGradientBoostingClassifier = HistGradientBoostingClassifier
ensemble.HistGradientBoostingRegressor = HistGradientBoostingRegressor
ensemble.__all__ += ['HistGradientBoostingClassifier',
                     'HistGradientBoostingRegressor']
```
