# Tailwind CSS Flexbox Fractional Width Issue

This repository demonstrates a common issue encountered when using Tailwind CSS's fractional width classes within a flexbox container.

The problem occurs because fractional width classes like `w-1/2` are relative to the parent container's width. If the parent container has not been given a defined width then the `w-1/2` will likely not work correctly.

## Steps to reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Start the development server.
4. Observe the layout of the two divs inside the flex container.

## Solution

The solution is to add a defined width to the parent flex container. This allows Tailwind CSS's fractional width classes to work correctly.  This could either be in pixels, percentages or another unit of measurement.

## Additional Notes

This issue highlights the importance of considering parent container dimensions when using Tailwind CSS's fractional width classes in flexbox layouts.  Always ensure that your parent container has a defined width if you want your fractional widths to work correctly.