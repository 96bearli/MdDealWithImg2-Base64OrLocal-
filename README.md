# MdDealWithImg2-Base64OrLocal-
## What's this?
 Localization of image links referenced in markdown documents .
 And you have two options: 
 1. Save in Base64 format; 
 2. Reference local images).
## And How to use it?
 * Put the document you want to process in the folder "before".
 * Then run main.py.
 * You can find the new documents in the folder "output".
## Import
~~~python
import re
import os
import urllib.error
import urllib.request
import shutil
import base64
~~~
