## CSS Injection attacks
 
 While most firewalls and sophisticated scanning tools are busy searching for malicious scripts, SQL statements, and code they tend to overlook the <style> tag. One of the common uses of CSS in web pages is to ensure beauty with uniformity which can be an informational aspect on a web page. Suppose a developer wants to use various internal and external links in his web pages and wants to show a difference between the links such that the user knows which link will throw them out the website and which one will open within the website he may use code like this in his style sheet,
  
  ```
from flask import Flask, request

app = Flask(__name__)


@app.route("/home", defaults={"path":""})
@app.route("/home/<path:path>")
def catch_all(path):
    return "<html><body>your path "+path+"<link href='style.css' rel='stylesheet' type='text/css'/> </body>

app.run()

  ```
 
  - for example you add this payload : `%0A{}*{colored:red;}///`
  
  ![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)
