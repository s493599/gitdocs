# Узнать IP клиента

```python
from flask import Flask,   request
@app.route('/ip/')
def get_user_ip():
    ip = request.headers.get('X-Real-IP')
    return ip
```