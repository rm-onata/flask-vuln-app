## open redirect
 
 
 - This vuln can be exploited by attackers to redirect users to malicious websites, phishing sites, or other malicious content
  
 
 ```python
from flask import Flask, request, redirect

app = Flask(__name__)


@app.route("/")
def open_redirect():
    url = request.args.get('url')
    return redirect(url, code=302)


app.run()

 ```
 
 if you get this address
 ```
 http://127.0.0.1:5000?url=https://google.com
 ```
  opening the google page
