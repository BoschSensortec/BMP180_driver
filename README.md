## Table of Contents
- [Introduction](#intro)
- [Version](#ver)
- [Integration details](#integration)
- [Driver files information](#fileinfo)
- [Supported sensor interface](#interface)
- [Copyright](#copy)

### Introduction<a name=intro></a>
- This package contains the Bosch Sensortec MEMS pressure sensor driver (sensor API)
- The sensor driver package includes bmp180.h, bmp180.c and bmp180_support.c files

### Version<a name=ver></a>
- Version of bmp180 sensor driver is:
    * bmp180.c 		- V2.0.3
    * bmp180.h 		- V2.2.2
    * bmp180_support.c 	- V1.0.4

### Integration details<a name=integration></a>
- Integrate bmp180.h and bmp180.c file in to your project.
- The bmp180_support.c file contains only examples for API use cases, so it is not required to integrate into project.

### Driver files information<a name=fileinfo></a>
- bmp180.h
    * This header file has the register address definition, constant definitions, data type definition and supported sensor driver calls declarations.
- bmp180.c
    * This file contains the implementation for the sensor driver APIs.
- bmp180_support.c
    * This file shall be used as an user guidance, here you can find samples of
            * Initialize the sensor with I2C communication
                    - Add your code to the I2C bus read and bus write functions.
                            - Return value can be chosen by yourself
                        - API just passes that value to your application code
                    - Add your code to the delay function
        * Reading the sensor read out data

### Supported sensor interface<a name=interface></a>
- This pressure sensor driver supports I2C and SPI interfaces

### Copyright<a name=copy></a>
- Copyright (C) 2008 - 2015 Bosch Sensortec GmbH

