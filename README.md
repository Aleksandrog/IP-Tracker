# IP-Tracker
import requests

response = requests.post("http://ip-api.com/batch", json=[
#insert ip after query
  {"query": "195.216.219.87"},
]).json()

for ip_info in response:
    for k,v in ip_info.items():
        print(k,v)
    print("\n")



