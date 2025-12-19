

To install the RESTAPI please follow the steps below:

* Create a conda env

```bash
conda create --name fastapi 

```
* Activate the conda env and install pip

```bash
conda activate fastapi
conda install pip

```

* Install needed libraries

```bash
pip install -r final_req.txt
conda install scikit-learn==1.2.2
```

* Use hypercorn webserver to deploy the code 

```bash
uvicorn main:app  --port 8000 --reload

hypercorn main:app 

```

*****FYI  the sklearn is compatible with py 3.8 to 3.12
***** > and the typing lib needs to use 3.9 py and later

```
conda install python=3.9.21
```


* The resul is acessible here : http://127.0.0.1:8000/docs 