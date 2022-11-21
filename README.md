## Data Processing Part of UROP2022 Fall
**The raw txt files**

Due to the huge size of the raw .txt file bundle, the ```HKEX Reports``` folder can be found in this [link](https://drive.google.com/drive/folders/1-gYNQiw4G49-AK8UHM8iDOrmeZnJEckO?usp=sharing). You can fork this repository and download the folder directly to the project.

**The file structure of the generated dataset**:

textual data|label|time
:-----:|:-----:|:-----:|
the text|"F":fraudulent, "NF": otherwise|"yyyymmdd" the issuing date of the report containing this text

**The result of running the respective files**

``` missing_file_to_df.py``` : process the *F* files not originally included in the shared dropbox ("dropbox") by Allen. These files are collected manually, cleansed, and stored in 'HKEX Reports/Fraudulent/missing_files'

```non_fraudulent.py```: process the *NF* files included in the dropbox. They are stored in ```HKEX Reports/hkex_reports_annual``` and ```HKEX Reports/hkex_reports_semi-annual```. Note that all *F* files originally in the dropbox have been moved to ```HKEX Reports/Fraudulent``` already.

```given_file_to_df```: process the *F* files included in the dropbox. They are stored in ```HKEX Reports/Fraudulent```. 


