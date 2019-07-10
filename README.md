# Implementing Experimental

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
