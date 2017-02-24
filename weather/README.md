# cli-weather

## Description 

cli-weather allows you to check the weather without taking a step outside your development environment. You can check the weather, directly on your terminal.

![](https://www.google.fr/search?q=cli+weather&safe=off&espv=2&biw=1366&bih=638&source=lnms&tbm=isch&sa=X&ved=0ahUKEwiNufCQkKnSAhVqJ8AKHWMICtYQ_AUICSgE#imgrc=N6U0NkmSXrQVtM:)

## Install 

```bash

$ npm install cli-weather -g

```

## Using

You have two ways to lounch cli-weather.

```bash
$ cli.js 
```
in that case, as you don't add options, the results will be by default the weather of dhaka in Bengladesh

```bash
$ cli.js "city" "country"
#by exemple: cli.js Paris France
```
in that case, the results will be the weather at paris in France (cf Explanation/index.js for more informations)


## Explanation 

### index.js

```
this is the file who call the querys. There is 2 querys, in function of, if there is an option or not.
if you want to the the weather in a particular place, you have to give option like city and country (in that case this is the 2nd query)
otherwise, the first query will be execute with bengladesh and dhaka like options.

```

### cli.js

```
cli.js is a file that is need to be execute in the consol to start the cli-weather.

in this file, there is the API meow which is called when cli.js is executed.

it will call the file index.js to do the querys and prompt the results. This is in this file that the options are interpreted (like F/C for celcius of farenheit)
```

## Options

there is 3 arguments possible during the execution.

```bash
$ cli [city]
#to indicate the city you want

$ cli ? [country]
#to indicate the country you want

$ cli ? ? [C/F]
#to indicate if you want the temperature in celcius or in farenheit
```

	

