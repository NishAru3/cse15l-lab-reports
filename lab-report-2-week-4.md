### Lab Report 2
**Three changes to the markdown parser to create better implementation.**

1. [Change 1: Infinite Loops](#1)
2. [Change 2: Text Inbetween](#2)
3. [Change 3: Images](#3)

---

## <a name="1"></a> Change 1: Infinite Loops

![Change Screenshot 1](report2ss1.PNG)

- #### [Failure Inducing Input](https://nisharu3.github.io/cse15l-lab-reports/failure1.html)

- #### Symptoms
    ![Symptom Screenshot 1](symptomSSInfiniteLoop.PNG)

- The failure inducing input has a error in the markdown file link format. There is no ending to the last link, which causes an infinite loop in the while loop. That is seen in the symptom. To fix this, a series of if statements ending the search when the next necessary element isn't found was introduced.

## <a name="2"></a> Change 2: Text Inbetween

![Change Screenshot 2](report2ss2.PNG)

- #### [Failure Inducing Input](https://nisharu3.github.io/cse15l-lab-reports/failure2.html)

- #### Symptoms
    ![Symptom Screenshot 2](symptomSSTextBetween.PNG)

- The failure inducing input has text between the link and the url. This is not an actual link anymore, but the symptom shows that it actually does. To fix this, the consecutive placement of the parenthesis and brackets is checked for, for a proper link.

## <a name="3"></a> Change 3: Images

![Change Screenshot 3](report2ss3.PNG)

- #### [Failure Inducing Input](https://nisharu3.github.io/cse15l-lab-reports/failure3.html)

- #### Symptoms
    ![Symptom Screenshot 3](symptomSSImages.PNG)

- The symptom shows the url of an image in the result of markdown parse. However, this result should not show up, as markdown parse is looking for link URLS. This is due to the exclamation point at the failure inducing file, and accounting for it to ignore images was the solution above.

---
Back to the [homepage](https://nisharu3.github.io/cse15l-lab-reports/)