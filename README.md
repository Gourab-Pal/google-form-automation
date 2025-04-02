# 🚀 Selenium TestNG Automation for Google Form

![Selenium](https://img.shields.io/badge/Selenium-4.0+-green?logo=selenium)
![TestNG](https://img.shields.io/badge/TestNG-7.0+-blue?logo=testng)
![Java](https://img.shields.io/badge/Java-11+-orange?logo=java)

A **robust and scalable** automation testing framework using **Selenium WebDriver, TestNG, and Java**. This framework automates Google Form edits and validates form responses.

---

## 📌 Features
- ✅ **Automated form filling and validation**
- ✅ **Uses WebDriver Manager for seamless browser setup**
- ✅ **TestNG for test execution and reporting**
- ✅ **Explicit waits for reliable test execution**
- ✅ **Modularized Wrappers for reusable actions**

---

## 📂 Project Structure
```
selenium-testng-framework/
│-- src/
│   ├── demo/
│   │   ├── TestCases.java  # Main test script
│   │   ├── Wrappers.java   # Utility functions
│   ├── resources/
│   │   ├── chromedriver    # WebDriver (if needed)
│   │   ├── logging.properties # Logging configuration
│-- build/gradle  # Project dependencies 
│-- README.md  # Documentation
```

---

## 🛠️ Installation & Setup
### 1️⃣ Prerequisites
Ensure you have the following installed:
- **Java 11+** [(Download)](https://adoptium.net/)
- **Gradle** [(Download)](https://gradle.org/install/)
- **Chrome Browser** [(Download)](https://www.google.com/chrome/)
- **VS Code** *(Recommended for development)*

### 2️⃣ Clone the Repository
```sh
git clone https://github.com/Gourab-Pal/google-form-automation.git
cd google-form-automation
```

### 3️⃣ Set Up Dependencies
Add dependencies in **build.gradle**:
```sh
  dependencies {

    testImplementation 'org.testng:testng:6.9.10'

    // https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java
    implementation 'org.seleniumhq.selenium:selenium-java:4.21.0'
    implementation 'io.github.bonigarcia:webdrivermanager:5.7.0'

}
```

---

## ▶️ Running the Tests
Run the test cases using **TestNG**:
```sh
./gradlew test
```


---

## 📝 Test Case Overview
The main test case `testCase01` performs the following actions:
1. Opens a Google Form.
2. Fills in text fields.
3. Selects a radio button.
4. Checks relevant checkboxes.
5. Selects a dropdown option.
6. Inputs a date and time.
7. Submits the form.
8. Verifies success message.

**Assertion Check:**
```java
Assert.assertTrue(successMessage.isDisplayed());
Assert.assertEquals(successMessage.getText(), "Thanks for your response, Automation Wizard!");
```

---

## 🏗️ Contributing
Want to contribute? Follow these steps:
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature-branch`)
3. **Commit** changes (`git commit -m 'Add feature'`)
4. **Push** to GitHub (`git push origin feature-branch`)
5. **Create a Pull Request** 🚀

---

## 📜 License
This project is free to use.

---

## 🔗 Useful Links
- 📘 [Selenium WebDriver Docs](https://www.selenium.dev/documentation/)
- 📘 [TestNG Docs](https://testng.org/doc/)
- 📘 [WebDriver Manager](https://bonigarcia.dev/webdrivermanager/)

---

### 🚀 Happy Testing! 🧪

