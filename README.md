# GEE
Interactive web mapping with Django and Google Earth Engine.
A web map where the user can view different vegetation indices of different satellite imagery.
Currently, only MODIS images are on display.

#### User stories: 
* Toogle between NDVI and EVI 
 
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
To run this project you will need to install Python3,have a google earth engine account and any code editor tool 

```
e.g Atom or VS code
```

### Installing
#### Cloning the repository:  
 ```bash 
https://github.com/JoyChristine/gee
```
#### Navigate into the folder and install requirements  
 ```bash 
cd gee
pip install -r requirements.txt 
```
##### Install Virtual environment
 ```bash 
 python3 -m venv virtual
```  
##### activate Virtual  environment 
 ```bash 
source virtual/bin/activate  
```  

##### Install Dependencies  
 ```bash 
 pip install -r requirements.txt 
```  
##### Initialize the GEE API 
 ```
 earthengine authenticate
 ```

 ##### Setup Database  
  SetUp your database User,Password, Host then make migrate  
 ```bash 
make migrations
 ``` 
 Now Migrate  
 ```bash 
 make migrate 
```
##### Run the application  
 ```bash 
 make
``` 
The application opens up on `127.0.0.1:8000`. <br>
If you want to use new server run e.g 9000
```bash 
 make 9000
```

## Running the tests

 ```bash 
 make test
```

 
## Built With

* [Python3.8](https://www.python.org/)  
* [Django 4.0.4](https://docs.djangoproject.com/en/4.0/)  

## Contributing
To contribute to this project, fork the repo, create a new branch then develop on that branch

## Authors

* **[Joy Christine](https://github.com/JoyChristine)** 



## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
