# CSS `calc()` Issue with Percentages in Media Queries

This repository demonstrates an unexpected behavior of the CSS `calc()` function when used with percentages inside media queries.  Specifically, the calculation doesn't seem to correctly interpret the percentage relative to other elements.  The `bug.css` file contains the problematic code, while `bugSolution.css` offers a potential workaround.

## Problem

The issue lies in attempting to calculate a width that involves both viewport width (`vw`) and a percentage of another element's width.  The percentage calculation within `calc()` does not resolve as intended within the media query context.

## Solution

The solution involves separating the percentage calculation and applying it as a separate rule using a different approach such as using JavaScript.