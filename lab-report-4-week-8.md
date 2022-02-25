### Lab Report 4
**`MarkdownParse.java` Comparisons**

1. [Group Links](#1)
2. [Snippet #1](#2)
3. [Snippet #2](#3)
4. [Snippet #3](#4)

---

## <a name="1"></a> Group Links

[Our Group](https://github.com/eNebulas/markdown-parse)

[Their Group](https://github.com/mBookUCSD/markdown-parse)


## <a name="2"></a> Snippet #1

*The Snippet Preview*

![Screenshot 1](report4ss1.PNG)

*The `MarkdownParseTest.java` method*

![Tester 1](report4ss4.PNG)

*Our group's results*

![Our Results 1](report4ssmine1.PNG)

*Their results*

![Their Results 1](report4sstheir1.PNG)

*Code Change Follow Up*
Snippet 1 deals with inline code that contains backticks. This change would not require massive changes in the code since there are only a couple additional if-statements needed. Looking into the brackets and parenthesis finders to account for excess special characters is not that hard.

## <a name="3"></a> Snippet #2

*The Snippet Preview*

![Screenshot 2](report4ss2.PNG)

*The `MarkdownParseTest.java` method*

![Tester 2](report4ss5.PNG)

*Our group's results*

![Our Results 2](report4ssmine2.PNG)

*Their results*

![Their Results 2](report4sstheir2.PNG)

*Code Change Follow Up*
Snippet 3 deals with nested parenthesis, brackets, and escaped brackets. This code change is much more intensive because the testing for each of these requires a stack of open and close situations that is accurately defined. This would need new loops, if statements, and/or data structures altogether.

## <a name="4"></a> Snippet #3

*The Snippet Preview*

![Screenshot 3](report4ss3.PNG)

*The `MarkdownParseTest.java` method*

![Tester 3](report4ss6.PNG)

*Our group's results*

![Our Results 3](report4ssmine3.PNG)

*Their results*

![Their Results 3](report4sstheir3.PNG)

*Code Change Follow Up*
Snippet 3 deals with new lines within bracket and parenthesis pairs. This is once again a heavily involved change because new lines require things to be saved in a similar way to nested pairs. The new lines introduce a different way to scrubbing through the file that isn't currently implemented.

---
Back to the [homepage](https://nisharu3.github.io/cse15l-lab-reports/)