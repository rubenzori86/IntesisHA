# pyIntesisHome
This project is a python3 library for interfacing with the IntesisHome Smart AC controllers.
It is fully asynchronous using the asyncio library, and utilises the private API used by the IntesisHome mobile apps.

## Usage
  - Add to your  <conf_dir>/configuration.yaml
  
intesishome:
  username: !secret intesisuser
  password: !secret intesispass

  - Create or edit your <conf_dir>/secrets.yaml with (mantain quotes):
intesisuser: 'username'
intesispass: 'password'

  - upload to your <conf_dir>/custom_components folder (create if not exist)
  intesishome.py
  climate/intesishome.py
  
 Restart your homeassistant server and look for your climate.* device

