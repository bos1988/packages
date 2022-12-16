# packages
selfmade packages for python

1. dsbudin - pack for data analysis and machine learning projects:
    - eda.py (ex base.py)
    - ml.py
    - timeseries.py
    - formattext.py
	- translate.py

### what's new:
#### v0.2.0:
- the LANG variable
- English is the default language
- you can switch to Russian (for this set LANG='RU')
#### v0.2.1:
- in functions get_research_test_m_ohe() and get_research_test_m_oe() added attributes `test_size` and `random_state`
#### v1.0.0:
- Renamed the `base` module to `eda`
- Module settings are made in `options`: `ml.options`, `eda.options`
- Added general `FONTSIZE_LABEL` setting: `options.FONTSIZE_LABEL`
- Added general `FONTSIZE_TITLE` setting: `options.FONTSIZE_TITLE`
- Fixed calculation of the `fraction` column in the function `na_info` from dsbudin.eda
- Removed the default parameter n_jobs from the `ascending_grid` function from dsbudin.ml
- Removed function `make_df_major` from `from get_research_test_m_ohe` and `get_research_test_m_oe` functions from dsbudin.ml. And, accordingly, the `features` parameter is removed
- The style of the correlation graph (`print_corr` function) has been changed
- Added function `print_scatter` in dsbudin.eda
- Added the ability to output a graph of the theoretical distribution from the `Scipy` in the `hist_box_describe` function from dsbudin.eda
- Added `translate` module
- Documentation has been added to each module and the names of some parameters have been replaced with more native ones