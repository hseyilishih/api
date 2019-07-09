# api_func.py

from flask import Flask,jsonify
import test  #my .py name
app=Flask(__name__)

@app.route("/<param>")
def myfuncname(param):
	ret = test.func(parm)
	return jsonify({'data' : ret})

if __name__=="__main__":
	app.run()
