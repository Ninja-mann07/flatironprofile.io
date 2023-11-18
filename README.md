import urllib.request, json

def get_repositories(org):
       “*”List all names of GitHub repositories for
       url = ’https://api.github.com/org/' + org +
       request = urllib.request.Request(url)
       response = urllib.request.urlopen(request)
       data = json.loads(response.read{}.decide()}
       return [repo[’name’] for repo in data]
       
