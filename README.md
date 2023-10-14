
# selenium in nodejs

Belajar tentang Selenium

1. poc Selenium





## Used By

This project is used by :

- Personal research



## Description about code 

kode somple 

```javascipt
    
    // call library for selenium webdriver 
    const webdriver = require('selenium-webdriver'),
        By = webdriver.By,
        until = webdriver.until;

    // using chrome drive 
    const driver = new webdriver.Builder()
        .forBrowser('chrome')
        .build();

    // type goolgle.com in browser
    // type webdrive 
    // check the tiltle
    // exit 
    driver.get('http://www.google.com').then(function(){
    driver.findElement(webdriver.By.name('q')).sendKeys('webdriver\n').then(function(){
        driver.getTitle().then(function(title) {
        console.log(title)
        if(title === 'webdriver - Penelusuran Google') {
            console.log('Test passed');
        } else {
            console.log('Test failed');
        }
        driver.quit();
        });
    });
    });

```







