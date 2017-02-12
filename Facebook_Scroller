import time
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.support.wait import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
from selenium.webdriver.support.ui import WebDriverWait
driver = webdriver.Chrome('LOCATION OF YOUR CHROME DRIVER')
driver.get("https://www.facebook.com/")
user=driver.find_element_by_css_selector('#email')
user.clear()
user.send_keys('EMAIL ADDRESS')
password=driver.find_element_by_css_selector('#pass')
password.clear()
password.send_keys('YOUR_PASSWORD')
try:
    login=driver.find_element_by_css_selector('#u_0_q')
    login.click()
except:
    login=driver.find_element_by_css_selector('#u_0_p')
    login.click()
time.sleep(10)
while True:
    print('document.body.scrollHeight')
    driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
driver.close()
