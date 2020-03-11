Results of EDA are avaliable on [Public Dashboard](https://app.powerbi.com/view?r=eyJrIjoiY2U2MTc1YWItYzc1Yi00ZjMzLTg4MjgtMTZhOTdjMmE4ZjEyIiwidCI6IjI4OGJmYmNmLTVhYjItNDk2MS04YTM5LTg2MDYxYWFhY2Q4NiIsImMiOjl9)

#
Data preparation was made in Google Colab  
Notebook for that is **data_overview_and_preparation.ipynb** in  repository root

**eda.pbix** file is stored on shared [Google Drive Folder](https://drive.google.com/drive/folders/1--WQpT7uSF5t0xQJB_LDXWdoYM4XInIR) and already contains all data and visualizations settings

#
To reproduce:
1. Import public dataset directly to Power BI
```
Power BI -> Get data -> More -> Database -> Google BigQuery -> bigquery-public-data -> iowa_liquor_sales -> sales -> Load -> Import -> OK
```
2. Run **data_overview_and_preparation.ipynb** in [<img src="https://colab.research.google.com/assets/colab-badge.svg">](https://colab.research.google.com/github/newturok/softconstrust_test/blob/stage/data_overview_and_preparation.ipynb) with yours **project_id** (Can be found in [Google Cloud Console](https://console.cloud.google.com/home/dashboard)) to prepare mappings
3. Import prepared mappings from Big Query private datasets that are prepared on previous step
```
Power BI -> Get data -> More -> Database -> Google BigQuery -> project_id ->  mappings -> specific_mapping -> Load -> Import -> OK
```
#
*Optional:*
- Custom map uses **IA-19-iowa-counties.json** mapping from [Google Drive Folder](https://drive.google.com/drive/folders/1--WQpT7uSF5t0xQJB_LDXWdoYM4XInIR)
