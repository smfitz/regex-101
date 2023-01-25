# Regex Tutorial for Finding/Validating an IP Address

As I approched this topic of "Regular Expressions" I quickly realized I had to step away from thinking of finding a solution though programing with a traditional programing language. Instead I had to look at the subject as an *almost completely different topic with different rule sets of rules that weren't limited to a specfic programing language. Instead it is a tool for developers that you can create using any text editor, to aid in finding specfic strings or forms of data. This was a confusing topic for me to delve into but I hope after reading my "cheat sheet" that you can gain a better understanding of what regex is and how it can help with many tasks. 

## Summary

As stated in <a href="https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial" target="_blank">The Full-Stack Blog</a>, "JavaScript has many useful methods that can check if a string contains a certain letter or phrase." Knowing only this going into this tutorial I knew I would be creating some kind of Regular Expression thats main purpose was to find a match based on a input. This is where I started to step away from what I was more comfortable with attempting in JavaScript and instead thought of a useful functionality I could create using Regular Expressions and could possibly use in the future within my own personal projects. Although not yet useful to me in any of my own projects, I took more interest in creating a regex that could find/validate an IP address. This cheat sheet will cover basic concepts of regular expressions with a more tailored approach to my specfic regex. This is what my final result looked like:  

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

Regular Expressions are considered a literal. This means that any defined pattern has to be wrapped in "/" characters. 

### Anchors

Anchors in RegEx are used to define what a string can contain. There are two ways of defining this as well as two characters that are considered anchors, ^ and $. The first way is to define an exact string with the carrot symbol. If I had a regex containing ^Dog anything that starts with "Dog" will be passed. "dog" would not be passed because regex is case-sensitive. The next way is to use brackets that define a range of possible character matches. A simple example of a range that will allow any length of a string with lowercase alphabetical charachters is: [a-z]. Using brackets also makes it simple to deine numeric ranges as well. To add any numerical value to the list simply put it directly after the first range: [a-z0-9]. The $ anchor signifies a string that ends with the characters that precede it. So if we were to define our regex as /^[a-z0-9]$/, this would allow any length of string that contained any numbers in any given order. Including the ^ symbol inside the bracket would find any string EXCLUDING the characters inside the brackets. /[^aeiouAEIOU]/ would search only for strings that contained no upper or lower case vowels. When passing values into a bracket expression, the value will only need to match ANY of the requirements inside the regex not ALL requirements. 

### Quantifiers

Quantifiers set the limit of a string, hence the name. Defining the quantity of characters inside your string is done through defining a set of numerical values. For example, {3-16} will only allow strings that are between 3 and 16 characters long to pass through the regex. They are inherintly greedy meaning they match as many occurrences of paticular patters as possible. Curly brackets can provide different ways to limit how matches work in quantifiers. For example, { n } matches the pattern exactly n number of times, { n, } does the same thing but it has to match AT LEAST n number of times. And finally like in our example earlier, { n, x } matches the pattern from a minimum of n number of times to a maximum of x number of times. Each of these can be made lazy, meaning that if you add the ? quantifier, the pattern will be matches as few times as possible. 

### OR Operator

The OR Operator is like a very inclusive and broad if/else if conditional in JavaScript. It is represented by the "|" character and can be used to define what different inputs can and cannot equal. For example: 

### Character Classes



### Flags



### Grouping and Capturing



### Bracket Expressions



### Greedy and Lazy Match



### Boundaries



### Back-references



### Look-ahead and Look-behind



## Author
#### - Sean Fitzpatrick
My Portfolio: https://smfitz.github.io/Challenge-2-portfolio/
##### GitHub: https://github.com/smfitz
##### Linkedin: https://www.linkedin.com/in/sean-fitzpatrick-220bb924b/
##### Email: s3an.m4l.f1tz@gmail.com
