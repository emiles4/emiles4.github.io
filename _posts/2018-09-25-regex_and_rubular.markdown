---
layout: post
title:      "REGEX and Rubular"
date:       2018-09-25 19:20:05 -0400
permalink:  regex_and_rubular
---


I recently completed the REGEX lab, and I had a lot of fun playing with the Rubular expression tester/editor. I have always been curious abou the code that lives behind functions like email verification and phone number verification. 

I watched a lab walkthrough that went a little further into the uses and methods for regular expressions, and the puzzle-like challenges where I could go from a blinking cursor to /(?<=\.) {2,}(?=[A-Z])/ and actually understand it was incredibly satisfying.

A Regular Expression (regex or regexp) is a tool that can be used in almost all programming languages,with a few tweaks. They are used to extract information from text (strings of data) by defining search criteria in a pattern. Each character in the pattern is a sort-of wildcard that when used together helps save a programmer a lot of time. For example, a regex can be used to find and replace text in a document, validate data, or to scrape data for a certain set of words.

For example, if you need to search a set of data for the single numerical character "5", your regex looks like this:

/[5]/

If you want to match a username, the below is one way you could do that:

/^[a-z0-9]{3,9}$/

Breaking that down into it's parts:

// - These are at the beginning and end, and are the delimiters that surround every regex

^ -  Finds the beginning of the string

[a-z0-9] - Looking for lowercase letters a-z, and numbers 0-9 ONLY (Uppercase letters won't match)

{3,9} - Limits the length of the string, between 3 and 9 characters

$ - The end of the string

Medium.com has a great article with a cheatsheet that I found really helpful in breaking down the types of topics that can be used, such as Anchors, Quantifiers and Character Classes. <a href="https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285"> Medium Regex Tutorial </a>

Tools like Rubular and RegExr are fun to mess around with, and awesome resources for quick reference guides for the syntax of a regex.
