# Unexpected Overflow with Tailwind's w-1/2 Class in Constrained Parent

This repository demonstrates an uncommon issue with Tailwind CSS's fractional width classes (`w-1/2`, `w-1/3`, etc.) when used within a parent container that has a limited width.  The child elements can overflow the parent if the parent's width is not large enough to accommodate the fractional widths.

## Bug Description

The `w-1/2` class, intended to make an element occupy 50% of its parent's width, behaves unexpectedly when the parent has a constrained width.  In such cases, the child elements, despite having `w-1/2` applied, can overflow their parent container.

## Solution

The most common solution is to use a flexbox or grid layout to manage the width of child elements within a constrained parent.  This allows the child elements to share the available space more effectively.