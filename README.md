# Space project  
## Quick start  
1. Please, register at [http://data.regional.atmosphere.copernicus.eu/openwis-user-portal/srv/en/user.register.get](http://data.regional.atmosphere.copernicus.eu/openwis-user-portal/srv/en/user.register.get) and confirm your email.  
2. Locate to the src folder in this repository or just rewrite `main.py`.  
3. Examples of data loading:  
```python
import copernicus

api = copernicus.API('your-email', 'your-password')

api.get_data(
    'ENSEMBLE-FORECAST', 'CO', '2019-03-21T00:00:00Z', 1000, 'Ukraine',
    '2019-03-21T02:00:00Z'
)
```