# NekoCAS_Python_SDK
NekoCAS SDK for Python

## Installation
```
pip3 install NekoCAS
```

## Begin to use
```python
# Input the NekoCAS URL and the service secret.
cas = NekoCAS.CAS("https://cas.n3ko.co", "vNOZpKdqnUYcztBjUhvvPLpeYCIIBVev")

# Validate the ticket.
user, err = cas.validate("ST-oadwZVbq5lUy151InUCC6UHDLI2l586k")
if err is not None:
    print("invalid ticket")
else:
    print(user['name'])
```

## User data
```python
{
   'name': r['data']['name'],
   'email': r['data']['email'],
   'token': r['data']['token'],
   'message': r['message']
}
```

