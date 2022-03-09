# Setup Instructions

## Steps

1. clone/grab the sample_site folder
2. make sure the folder inside sample_site is `templates/` with an `s` (just in case something changed)
3. create the python `virtual environment` using `venv`
4. activate the `virtual environment`
5. now we can install the python environment libraries with `pip`
6. at this point you already have the files from lab (double check):
   - count.txt
   - requirements.txt
   - app.py
   - Procfile
   - templates/index.html
7. 


## Commands to run

1. python3 -m venv venv
   - this assumes that the `python` version you are using (and saved as) is `python3`
   - `venv` is the command to make the virtual environment
   - we name our venv `venv`
   - think of `-m` as to make the `venv`

2. source venv/bin/activate
   - this is for `Unix/Linux/Mac`

3. source .\venv\Scripts\activate
   - this is for `Windows`

4. your terminal should look like this (`Windows`):

``` Terminal
(venv) Path\to\sample_site\
```

5. pip install flask gunicorn
   - maybe you use `pip3`
   - maybe you need to setup `VS Code` a bit more first (this will be in the video)

6. we already have the files but you can also generate a `requirements.txt` to ensure your app is running the proper python library versions with:
   - pip freeze > requirements.txt  (might just work for `Linux` I'll double check `Windows` later)


## Test the app

1. To check the visual content of the `index.html` file we just drag the file from our folder to a browser (or `open with` and select a browser)
2. To check the app itself with the local server we do the following:
   - run the app with (use your python version same as before): 
     - python3 app.py 
   - open a browser window and type the following as a `URL` (both options do the same thing so only need to use one):
     - localhost:5000
     - 127.0.0.1.5000
     - (localhost _is_ 127.0.0.1)
3. To check the app after deploying on `Heroku`:
   - type the `URL` you are given from `Heroku`
   - in my case I named the app `eecsweb` so I use the `URL`:
     - [https://eecsweb.herokuapp.com/](https://eecsweb.herokuapp.com/)
