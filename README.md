# Extract-email-from-a-website-using-Python
How to extract email from a website URL using Python

In this post we will learn how to extract email addresses from a specific website or a URL using Python Programming Language. Here we are using regex and request module.

### Module Installation Code
```python
pip install requests
```

Extracting Code
```python
import re
import requests

url = "https://www.techcvr.net/contact-us/"
EMAIL_REGEX = r"[\w\.-]+@[\w\.-]+"

r = requests.get(url)

for re_match in re.findall(EMAIL_REGEX, r.text)"
    print(re_match)
```

DONE & ENJOY
