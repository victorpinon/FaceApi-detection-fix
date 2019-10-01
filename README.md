# FaceApi-detection-fix
Fixing Azure Face API Python quickstart guide errors

Based on [this guide](https://docs.microsoft.com/en-us/azure/cognitive-services/face/quickstarts/python-sdk#display-and-frame-faces)

Fixes the following errors:

```
Traceback (most recent call last):
  File "azure-face.py", line 40, in <module>
    response = requests.get(img_url)
NameError: name 'img_url' is not defined
```

```
Traceback (most recent call last):
  File "azure-face.py", line 46, in <module>
    draw.rectangle(getRectangle(face), outline='red')
  File "azure-face.py", line 32, in getRectangle
    rect = faceDictionary['face_rectangle']
TypeError: 'DetectedFace' object is not subscriptable
```
