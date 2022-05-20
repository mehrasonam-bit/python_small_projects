#import packages
import os
import requests
import json


url = "https://moviesdb5.p.rapidapi.com/om"

querystring = {"t":"the batman"}
#hidden the api key using Replit 
headers = {
	"X-RapidAPI-Host": "moviesdb5.p.rapidapi.com",
	"X-RapidAPI-Key": os.environ['api key']
}

# there is inbuilt json() constructor for requests.get() method
response = requests.request("GET", url, headers=headers, params=querystring).json()

print(response)
# To actually write the data to the file, we just call the dump() function from json library

with open('movie.json', 'w') as json_file:
    json.dump(response, json_file)
