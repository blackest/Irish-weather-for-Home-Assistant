# Irish-weather-for-Home-Assistant
A Simple use of the rest sensor to get the short term forecast for Ireland into home assistant
Home Assistant allows you to create sensors from data available on the internet. This Yaml file creates a Single sensor which stores the data as attributes The second half of the file creates further sensors which use the attributes as states which can be displayed recorded and acted on. 

In the frontend of HomeAssistant you need to create a dropdown list with at least 1 county in it You could use a text entrybox instead  once that is done you can make a card in the front end and do something with the data. 
To use this you could add this into configuration.yaml but better is to put it into a folder called integrations just ensure that you have

homeassistant:
  packages: !include_dir_named integrations
  
at the top of your configuration.yaml file   
and from this point forward you can create a new yaml file in your integrations folder for each additional thing you want to add to your configuration.yaml file.
mixing up different integrations in configuration.yaml is bad and can cause hard to fix bugs and stop existing integrations from working.
Hope you have fun with this and it helps you get started writing your own restful integrations.
