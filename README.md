# Web Semantic Editor
A student project which target was creating a text editor with context menu and modules to it like: text statistics, speech parts, synonyms.

**GUI**
![alt text](https://github.com/BartoszWlazlo/Web-Semantic-Editor/blob/master/readme/GUI.png)
**Text modifications after turning text analysis**
![alt text](https://github.com/BartoszWlazlo/Web-Semantic-Editor/blob/master/readme/output1.png)
**Examples of found ontologies**
![alt text](https://github.com/BartoszWlazlo/Web-Semantic-Editor/blob/master/readme/outputlist.png)

### 1. Install:

* [Python](https://www.python.org) - 3.5.X version

### 2. Download all files from repository.

### 3. Open CMD-Commend Line as Administrator.

### 4. Write:
```
pip install flask  
```
```
pip install owlready2
```
```
pip install nltk
python
import nltk
nltk.download()
```

### 5. Go to directiory of app.py for example:
C:\Users\USER\Documents\GitHub\Web-Semantic-Editor-BACKEND

### 6. Write:
```
python app.py
```
Wait for app to show http://127.0.0.1:5000/ then go to this adress.

## NOTE 1
If you want to change ontology you will need to place it in Web-Semantic-Editor-BACKEND
and then change the name of ontology in app.py line -> 14 ->  

```   
onto = get_ontology("file://people.owl").load()
```
## NOTE 2
If you want to use new frontend build:
* Build frontend with npm run build
* Copy css and js folder from \Web-Semantic-Editor-FRONTEND\build\static\
  to Web-Semantic-Editor-BACKEND\static ...  *TIP: delete all folders in backend\static and then paste folders from frontend*
* Copy Web-Semantic-Editor-FRONTEND\build three files then paste it to Web-Semantic-Editor-BACKEND\templates\
