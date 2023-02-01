## OSRF (On Site Request Forgery)
 
 
 ```
from flask import Flask, request, redirect

app = Flask(__name__)


@app.route("/")
def on_site_request_forgery():
    vuln_param = request.args.get("vuln_param")
    return "<html><body><img src='http://127.0.0.1:5000/images/{0}.jpg /> '</body></html>".format(vuln_param)


@app.route("/admin/add")
def add_admin():
    user = request.args.get("username")
    passwd = request.args.get("password")
    return "Admin Added"


app.run()

 ```
 
 
 - the whole goal of this vulnerability application is to force the user to send a request to the "admin/add" endpoint. Foing so will cause the application to add an admin user which the attacker could use to login to the victims application.
 
 
 
