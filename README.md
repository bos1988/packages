# packages
selfmade packages for python

- **dsbudin** - pack for data analysis and machine learning projects:
    - eda.py (since version 1.0.0, ex "base.py")
    - ml.py
    - timeseries.py
    - formattext.py
    - translate.py
    - math.py (since version 1.1.0)

## what's new:

---
### v0.2.0:
- the LANG variable
- English is the default language
- you can switch to Russian (for this set LANG='RU')
### v0.2.1:
- in functions get_research_test_m_ohe() and get_research_test_m_oe() added attributes `test_size` and `random_state`
---
### v1.0.0:
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
---
### v1.1.0:
##### Bug fixes
- **general:**
    - Increased the size of some default charts
- **module `translate`:**
    - Fixed a language detection error in the `translate` function
- **module `eda`:**
    - Fixed a bug in the `get_corr` function
    - Fixed the regression line in the `print_scatter` function
    - Replaced the function name `get_corr` with 'get_corr_target`
- **module `ml`:**
    - Fixed passing *random_state=random_state* in the recursion of the `ascending_grid` function
    - The `reset_index` method in the `get_research_test_m_oe` function has been removed

##### Mods
- **module `eda`:**
    - Added attribute `min_corr` to function `print_corr`
    - Added information about duplicates in the data in the `start_information` function
    - Added the ability to sort output data for the `start_information` function
    - Added regressions on the graphs of the `target_corr_reg` function

- **module `ml`:**
    - Added attribute `test_index` to the functions `research_test_split`, `get_research_test_m_ohe', `get_research_test_m_oe`
    - Added attribute `func` to calculate the error in the function `print_predictions_type2`
    - Added attribute `drop_first` to the function `get_research_test_m_ohe`
    - Added attribute `nround` to adjust the accuracy of calculations in the function `ascending_grid`

##### NEW
- **general:**
    - New module `math`
- **module `eda`:**
    - Added `snake_to_camel` function
    - Added `show_corr_target` function
    - Added `set_true_int_for_float` function
    - Added anomaly search function `find_anomaly`
    - Added `NaFiller` class
---


